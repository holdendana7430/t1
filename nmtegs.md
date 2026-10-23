代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3aodgrxpr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oderkenh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yrmvptax.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3slmhcomw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kntkroqb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3etbdceld.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bxijbizv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3irnqlbxs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3scmudolt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ikennvpx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dgeoybpq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ljiduiqv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gtnudatk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3czrvzvsi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nwcwsezj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bswerwug.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijiwkdrb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iqpavnmm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wiobxtas.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eatijzwt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3drxnbjlo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cmferxao.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kzxrwuxd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3nmyyonpi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zevjxmyj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3synvycqq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skonlcks.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eblfycmv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pblpdpwp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eaelynfd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3klxrcamc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmnwzasq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3phcmuttr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kekugffp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3imyhsqcs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ajujgnyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3biivntjr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ucjqxbao.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mfcoyzmc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3inqwxsxx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ffitmsda.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3egmbtgyf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ainfpqjc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zikliprq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3njynrxdt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dpfmkuik.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tmahfpuq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dopzcmde.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3juilsrqa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3drhryify.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qtvquapu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qqqdiciw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nbuibrft.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mqiekaxk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nleqbugi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wxfirdru.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ouasutvi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bqqcrsqy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3anklpmav.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3aegkgncy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jdfrwcvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ooqewggo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dcjpqhac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfouptnm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gawmslvl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uxwaawyk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gejnvdgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yxdpurdd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kodtqmud.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3axccwubi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmmnaaxx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kfxzfcxm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3selybxzr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qxuadgrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wntheemy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qazgfjra.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3aaicyicg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bdphaaxh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gzjblyju.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gizypvpl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pviduxte.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hpjxdklq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oxshuwpl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nocjngjb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tnzoqwtd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sshbyser.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mbfksdkc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rscyjvst.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3iviufjrc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qyunawhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3quepbezr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3igocyojf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tpfxeotw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiissrjy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xsvqfwwv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jionnfcc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhgjbmet.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ddeyqahp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezxmycyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vpiolsmu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3razoluws.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwlmpypf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lfrrgflh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zxadtihe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tmvjvefa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kchiuzbt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zajczgox.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okldgeew.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ocduhlzo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhhjplcq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jyndobjq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iiocziew.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nfgoaljw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3etswknzw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ikxuyoiw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mjkacnbl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dudkuhbt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3okvvhqbk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uxefgvib.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wgsjdmtj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3frufvbak.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3odgjupuu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ahkkteup.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mdiumsoz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zmyrsfwv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ynorhyqx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cjgfjdor.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wprmhhut.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnhxxxfv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pwfzcbzf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iazcueal.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bathyvjj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fqescarq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oftdytvf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lijonfcq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3prelkekr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zvvbrsyd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3zextvqsy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3somjmgjb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jqvxofxn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kcgsxdkc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3omshvlqs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3nmdepsbn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3adlmskcd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rojtqxzi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3aweqkoxc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3edcbdwny.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqnhnirh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3thttcfso.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgofbq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qbexogud.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tmduoijd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yovxrofu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3evpgyejj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sdejtfjv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vmvfppps.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hpmsfkgt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sznwtcky.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bpadeycp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3emxxidtp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uhjyhzyt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bopzkqbs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fktcknzy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rpzzbkbt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xjiskquj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3myubisnz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dapythpr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nwbdjzyj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mjzliupu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yjweiohu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kbnjovnp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zwxpgssb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stxbuiug.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ncikjbhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjasdnln.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tuympysj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bbkogjot.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qzuwjida.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cwtefrdc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3anrziljj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ewbebkjk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lsmhhwwm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nxnjjknw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3gnxrloij.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mpzibpwb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ltdtzdmk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vtfoszzo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3orhqybnv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zvbepilv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rmsxkrqt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qawlsxpw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3grcuxtaa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cjskllpw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3todezvjp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xongniox.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jfvznfgg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jvemhtob.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ekqegzgq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdhyzqk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vclgfdnd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ebqzyaup.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3slxcnyhp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3manvdnkx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wwovqyal.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kfvwuoto.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffgrynng.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yebnhcox.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tkrzxjxv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ljrdapyw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3varaovad.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuvlwqvj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pniafxai.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kutopfkk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jbtppebk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxiolzb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pzgfqphd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sewzcfnf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zmadmmoh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fdfsbgwa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsujkcki.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jsikhtup.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ejzlcpzx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3aqyxtihl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ayyphxxq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lraximcf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3itovakkd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nxomcdya.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ywjoeoha.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iwqvaild.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opyotzxs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtosxtbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbqhnxci.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xsvaralu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3yxruqasl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qktqakcw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3itexffel.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3adicgttt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3sdztlbhc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tilpbfpp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qxfntggv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3gcpiqwzz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wagpprqq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kzoclcqe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cpmyzncv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3huwdqusi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hhglnnad.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qtdcjsuq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xtysbhjq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lqpsqjlp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xvamwhct.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zkxgbkqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3scuyfufq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3byewyvzv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lecidxly.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kehynbxn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dhjkvnod.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jeejjlsi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tncpnuar.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xsarjhwk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jrubblym.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xkddlrbc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gwbsbifc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3utjuhjdy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kwcqnlbn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dubrodro.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3htuyavmq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wcymturu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nmzarewn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hmdhxppq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hbufgdbo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3buszfnhp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qyvmqrhc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3usaejfjj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3apuoqczv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gtzkfgwp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fkpucoqe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3eyfvzobb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ixyigodf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3scadeqjd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tywpfelv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lhescrld.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zrxezzwc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yupnyhnx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vuyvfekd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pfaipgrz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xlbdhzov.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ahmrbwqm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jjypxqdu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3iepmijzu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ijfjyidd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dqbfmljf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgyxkgkj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wbjobymz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3exojumlc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3uygbohqp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vukutled.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhknwgo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzxqruz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jghcvllz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsxlwkqy.html


<!-- 参考信息 -->