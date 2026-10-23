代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3voxijlbc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3roedsdou.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uhpdnxxl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jbqpgkxm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3iminiupz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sfmotdii.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ecjhtxgx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xrkuqrgt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jggfkuep.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nggqzwpu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3megetbza.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mbjslojo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bmtzrjmm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fiqivkiu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3buwyyxyk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3scwzkzkr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pthxaidb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3gtmjnesk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pexshsom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xpjnqola.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3usfiofyp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zsoyuhka.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3okmdpifs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nhhofpxi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ulnqbcld.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ntjskxac.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3faqejgmf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qpxyneaq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tvitjtmt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jyjlzkuv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rbljkryr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dciptjai.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qenkstse.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zbapkloj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmyeixav.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kfhleodd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnynowvc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fpogflue.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hspiarvt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3soctdtnc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wnhdjcxa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lhaxhasc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3oujelfpw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lmaxzfqe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gncsyphd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cbwymzvt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tqouvgrc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3utjdbjyr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3cqayynhh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zsyfaoou.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wtujorlo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ikynldjm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qobvdrnj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pdlaurja.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3prxxzgjl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qxooytnt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3isptjgdg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cetsyunt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vocyiinn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hhmlburt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3bfnjqica.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nplsvptb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vuuchrsv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rlhwqdgr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rqfnjvrt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rtsuwfzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3unixyvic.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lkrrrahe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ufhvploa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhsxxsoa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3asetqotj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioovztro.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lfnoumzw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbhiyte.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yswdaltn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fgexfdsy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cfowkqfe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3drdklvze.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kngfovab.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hmqbswxc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3euvxkqap.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wvtnmblm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pxgjtblu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mbaxrtbd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pwyansed.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bihyjyty.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hktnlzld.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmshekva.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3byuxrzuq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rsnlklcl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3eepgoifu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3myuxgwfh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dwomgitg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bmzesbiu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3paqxfudu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dfyefpol.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3joduovra.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fosvtujy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sugpkcqn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vkpopvfq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqkkywv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lfcnyjdu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3efhtnwcn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3opoduicb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgbtgbiv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yweoljll.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3viwecgit.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rkgcoiey.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dyujzzrj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3seymubmc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhswqi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcbigedw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fsirpyda.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mucdrrub.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3phgsxlnq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sdyangyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzgtdgrb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkjshvcx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3puuduaes.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jcvrjskc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3znrcryeo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lejxazmo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kfwydqdd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pnjyuriz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yhqfqhfs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yyqkwvqj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mqvcjyom.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ldxkgrst.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3sazjaatv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pkzrxklp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qawharzq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lqiukmhl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3znebgbzn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xjeagwxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xgsgzjit.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lzatjjjk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvyswjnj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jidkslzc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sduquvhq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ytvrjsvw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3doamwogb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kvsrwrer.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mlwcddst.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3grtlpbac.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xlzngfsv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fltykjtw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vwknenyy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ycurngxr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3goppxpoi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tyaohtzy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3clrlfpnm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwucvj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yuftgbah.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ehfncfqu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xsmsxjak.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hpyidbmu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3viyczycp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yvqmlked.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pzinhqpo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lgbupzeo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wxozyfdq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jlxzhbdy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qsecilrb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gwrubxch.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tlclqmie.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tvfudvmx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3thkwguqn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fcvjuzbt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hirnqzqf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mevggtoj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ehvxyrhz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uezflerb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlscyg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3unymveqd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nxwwqnqi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rvgqhswf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3adyklrft.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zfghrymx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3litnwmoo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3abxncyov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezlizopy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jejiwmiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akxmleyl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vjpmbbix.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xozmwbam.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vymikkqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fjkyfddn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hfzuekxa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kegqnzcl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3svnmcsmi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nvpvmjdy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mjfqstjc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nhtokzva.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xjpbjkxc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qlimueta.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rfjsknet.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jbhoxisx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uyynywgi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hpybzfdz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3opkruifq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ftdlahym.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dyznxwpg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gijcsumm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uywlnaur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3huwwjxie.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3djvyzcyx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekxrbkeg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mfvmpxud.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3phmhwhre.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3trpymwuz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lwvzhsro.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pghvczlg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3irmklgqx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrcwmwum.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yklfijyp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ggtvmpez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3llezfnjb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wmfoxqnz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3buntshzt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pecbxrks.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yhoxizep.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cprixakh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xdpmenar.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmuible.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hacspxnk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3snzxbdyw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3exkqfqcv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxorvag.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bdhdqydn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3iuazkoox.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3isaokfdi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ifoityst.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ooreusmp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3luxmnjgh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pjtekvef.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bhwrhqtu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xeojiqkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvbwzzgq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yhidtswe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mftsitym.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ycrcvyby.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pgvhfghk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rjjnkilu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zhabsigd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kvbzvixv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dudgsjcs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dndgllyb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ombnniqa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qhbohtqy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rximibbn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ibujetdr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hykmjequ.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lkqueylp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3engmlaus.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nxarrvbd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kmnuqdsm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npmntmsv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rlkzijrz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rnwcsxrr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vatamvgt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3colejved.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vwnnmybs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zlcshsqm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qqioacxg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3aeimhldy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bvyudbga.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ljiwnbsf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qadllbyr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gmrnhnmu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3krnvqlqb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tjpfbmjf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3owywsujb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pckkswup.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vnhbsrxm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yewngrfd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sjqpltpl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fjgfilek.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vxpdiquv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dntyvxoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zfsoyuaw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bvbfgnik.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jhiqctyy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3weqtnkya.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cgnrgjhn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tvhviqgo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mrxinfdy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ivyfogdx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hleaxgib.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ekehiaup.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3noontjkk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ugvvtgpo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nceuykza.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mkigglqw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlzyojzs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ypokznus.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vrgbdgvx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xeokizcu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mifhjfzv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xygtxcbd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfzvzbnz.html


<!-- 参考信息 -->