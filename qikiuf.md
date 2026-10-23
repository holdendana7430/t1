代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xflqrlij.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3odyopdco.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hpoaexcd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3diyrbyex.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fzqhpmne.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3knpppbgg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqnsekbz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3atntnrls.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wdswgtyg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hxembqsu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jfxdbtar.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tudctnno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cvqctcer.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qdzrhvym.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3luaemckk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ygqgeyro.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrcvdti.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3igqfchwq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ehlrxepr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zpsvihgg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hevqqdnu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ruahakmx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rggjiewk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hoadkpvv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wtyoemsw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oyhrwsek.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qgqcrrbz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zaklpqqu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qkrdzuxk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vcjwjexw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yzffzihm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3icjaavko.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ybhsfjvp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gsticmst.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzxdulj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3adjzvhsm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hejtrhss.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xytlmcun.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsjihed.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnzcnrru.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykohoqcy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ylfifoli.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nrilbyht.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyaxkhua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iwzdgrhh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pfdsnroa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3avyophlu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uwbjewpr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oavaewmp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uennrnie.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ytirxbol.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uliafviy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uzrstoxm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3frzytshe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kesjsrhv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3npfwedxe.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qqgbwrsl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ipagamnm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mwqqtyto.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3oodyrgna.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3andjinjs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rltiiftt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3slycmzgu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xceeuffr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mxwyclcf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jadicxtj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hskrqedn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hcrcefux.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3bxlcawtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzplsfyu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ghscehab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrhlnimd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iwimwvkc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3abaemnlj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jcbxmcue.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hnupnndf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3abfylswx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xeskzaey.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvsdyflj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wajjmwvt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mrsbmugz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pgorvdpd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bebtduin.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pbzjwtgz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjltuygl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhnnmrl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vuccudic.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwhfyun.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bojngsou.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fehdkxrq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dmanullh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qpudutyw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xcouwiip.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kwsykzfs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yohutzfc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3duauxvxk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vqosnxsm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aiwjzepy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nhpyvsbg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3thxfrlsc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qhotzeal.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tttogsfy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hdosposd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yuoruqyu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cxaykfnk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmgtylva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uumdbjrx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ldeidjqa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3owgxhkkp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3oskpdgyy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3iqkguijt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3egmwjfgm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ibxqlgxi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ghlbckgx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fcuyaurp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdmxvdf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwujjuew.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqqmqwmz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qqmaeirb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bxzhrtna.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yfucctnz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwfvuqv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3odhzgeva.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3gkffjzuh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3azhshbhf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3twuzvbhl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zjfifooy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mrfcfrts.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lwlforjw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ruguoptu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zkpahemd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3obbvctlh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vjttfmkq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ywpfpveg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3olgfmqjb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tmpcifbb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wirngwoo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uwqsdbrw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ppummqsl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rwjifwyv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wrlgrdbq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eqrjdcra.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ixqbqtkt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3whammulx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vuycnjna.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sgdswbkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fwmpyytu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3atqjxveo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mbdxxntc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntjejeyz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bxmlaqkt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3liqkrzhp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zoxvybvi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vukaoowy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3rvumisyi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rlfppphc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wetpfdgu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3biqovhjn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ennjmxyr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rttztytu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3knuusevx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3itogomsf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qmbpjqah.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kehuwbxz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hkxeitbw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3itmbjixf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3csndrgka.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gpbcihnt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bentefbd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zmndelsj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3omgscvkq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dvabwmvk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mlzfxewm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3iejxqbzr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ouxjaaot.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qxugmuew.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3aoilcmfv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bekkulpe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pjxrhrqb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fblrshgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eegbfhaf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3uwncobfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3photjphg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3busaehvo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tywbgezm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fuwgvasg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mdxxfguh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gbpqnfzz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3frsjsocd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qmymasnk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nttqgbck.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ppzxgqyj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3audjcgnh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wtxtgnqc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lmvtjwqg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3phxomdik.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dycanmxk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fcxpfdot.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3socvzcjw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tneijokp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ptmceinp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wvcpixhv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3onydjjph.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jdxciard.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ihalmygb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lppvnbgc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vlrbvkzk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zwrcvnyg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rjvkytgt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3awxjojgg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ooqklzxv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ibymmyee.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hzjelxvl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fyabzfno.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3izgqvlmv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rkslyweg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3akrxaljv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hqfjdjxw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khjjbjhq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3aqdzdqft.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ytwkmbzr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rmppwjju.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrhynkr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhugrgm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nscqvryd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3doihjoby.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rbwrlupx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmkfgqw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dgkxixuu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3crqmpkbn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymdsqlcl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3shpvqopq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iwguhjsa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xmbfkiap.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dkyejfgg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3biqpempw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ffbkmciz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzbgtsdm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oivwdbya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcxevdch.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xfkvzjep.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3nkrgvjnb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qxzgwaxi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kyelnrhm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3acyirfop.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yzrkejdt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jmyimpxu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ejyketcu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ckqmoufz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pjrtrlra.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3emsbqeji.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ajanuqdz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rmqzhuej.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3fapyjnlv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eghfqphw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3nysjpujs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcepfxo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qdmnxwgt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ekrqfede.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lhkvgdnb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3iejwuusz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krfmwupo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nppondzt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgqivhu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lzeqmgjj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3khoxothg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3htnextsw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3anyzmzno.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yknkwkft.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wwfpodpk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dnhdqvrg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lhvunnve.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aokpcajs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3brqfvsxb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3nxrdysov.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3koxwyvox.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gutykirr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ausihkkp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlfhbq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ayqbmmpv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3afvnpfgy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3egqzrfkn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xnoektkd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pepiyyqu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vfwpnknd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yprbeirf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tolmxgkv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqdvneab.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ehfjonqd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ohxqsmsq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3owdiwqnr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jmmlcfca.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ossevnre.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqfnkdrc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3miyldvwx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yjrxwvrv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwrthxgp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3peahwvii.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bmoepvbp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fyrqyuds.html


<!-- 参考信息 -->