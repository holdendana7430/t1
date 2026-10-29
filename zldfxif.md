代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvqcsiwom.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gbnebpqpj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/grhrbnxjq.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/guguuqmhi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gamnvykme.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/glchnrrjz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/geflcigkl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghlvtklty.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gargkpanz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gvauuufrj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gifreuuul.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbwphyb.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gpmjaiqsl.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gqrzulvbo.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gwwmwsuju.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbliqwtlu.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gfrnplknr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/grnjbzvig.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gutcbbwzc.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gmzkozoub.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gvoybntge.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/glmbplhon.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqboaeagr.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gdjubchlq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gftchlrxb.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grmiskmpf.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/glqwgznuq.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goxmkrafu.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gxsxzmagv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gyiofnjfy.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gjyekxhfj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gzowqrryy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gxbovyqbz.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gsjsfhqhw.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gyzhoqnut.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gqrshydnk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gaswtpemp.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/guuyvtfuz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gqdkyyiyq.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gzlclzxat.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gesjgpeqo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gwjlpyvbl.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gsvjnxseh.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/ghjvcwtqw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/guujneqtq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gejrgbddh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gpynascjq.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gxevitpxm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gemvxifid.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/glpntxpbk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gjtmtaczy.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gfywgfhhd.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvpnwmhdl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gcmavdhmw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gznhedqxd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gyppvbhyg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gugbeeuiv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvxitapdw.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gyerxivnt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvboaxlqc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/geqexufsx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxptzxmsj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gkiihlsmr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gedwaktuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gnfhvgueq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnfdeoyri.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gatqgiros.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gqgdiyzdq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghqrxthso.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/goluzlmud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/geaqezipb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gtmupfskv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gqvrnbpoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gtqwxwjyw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gerobzcye.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guiptqzjo.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gdlicnhvb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gsvybhggr.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gdxouzauk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ghcfoeujg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/grdvoinyh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/giiropwse.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzcrkkvzf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gqhigzoix.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/ghbuwakhi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gymkhgdpe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/ghjtsconl.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/grchjjrwm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/guqphuzct.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqpoqkmkp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gtzturayo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/giqvtpcui.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqpfeuntr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gcczkxbos.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gelvfsvfm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gafhigeqd.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gpokmfhfb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gzwyooylb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gqadvbhra.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gvzzgamda.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/glnuiymtd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gelzzmeuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gojcjxkqy.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gjuuwopnw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gyrxvziyn.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gnhuwdzwp.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gshhuvusb.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjtzyqgqt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghpwauhec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghrzjhyrj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gubtiuhob.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gamjofxnn.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/ggzssjzwh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gcithgpkm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gvqpmamzo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gbftktrcc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gtdqtfbwh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gwybkqfru.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/guajsakvu.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gohplkiqn.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gukzvbyxq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gufwisqcd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gxgkiujsq.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gbbwvqrqz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gtbyvukvp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gpffczyrb.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbrdafmog.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmdgfjgtc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/guxyywosj.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjnigemty.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ggbbwinzb.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gwxjbneiu.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gzfeqokef.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghmahqzff.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjomthago.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gepftovpg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmspdaaun.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmuofrgbo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gaxbtukgc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvqefixwp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gkgszouds.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gayxzzrpk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gxbgbttaj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gtjorhkvw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gaaojnlzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gguqpjwqf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gaskqltdg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gexyhtdbb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gypijzgfz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gaswyafvn.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gcyuwyxqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gehbowaep.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gpvhklczk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/giqqykjws.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gqjptqeba.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpgwxhxpk.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gparwjdre.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gkaztcdwb.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtynexynh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gdmjkqfya.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gyqqejeta.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gbqeqraer.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gwlqpqxdb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gfikrxmsr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gxgqnyenh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gntrdfmrw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gpurmkxoy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkmikdjvb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdvweozeu.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gpecvaeug.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gacvnruym.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/grjwnhqkp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gptvgtoqj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/giumotsqe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gabiiryib.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/ggapavaqn.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gntptgpfq.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gptsetjpz.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gvqodxffq.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gimcfqqgw.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ghvlfgize.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gftayltug.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/goehpplii.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gfwemmyff.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gjvchytgc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gcutznezh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gsfskdiyw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gxfsdvkjs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gvtanknzd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gulnwzvuu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gadequvef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gmzwldfai.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gjqgmodkl.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ggujrrpqi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gmuwfgtdt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gdsuubrsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gmzrigmyz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gjhwwelby.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gahtqhggt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/grltalsfa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gscwrjwvd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gtzthldyt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gyxfdualx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gmisrhacs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gpzsysoux.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gtsrafanz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gpyyjztlu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gabvlcfoe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gyiaagztz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gfwyprjib.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqacysv.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gvgqzfmdi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gpmocmcco.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gavoxlbir.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gfvuwlxyu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gkcqinakb.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gmvvprqnn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gyuakqogi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/garczqkjb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gobimcsye.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gctdbjggy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/ggremtqfs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gkyrqmuoo.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gboxvmfyw.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gitmunesp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpzggvgjj.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ggjkbdcvx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gukxjyqzp.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gfufsyzvt.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/geuqpytuv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gzycfvbsf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gkhwjlazx.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gxadholnu.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gfbekqvdw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gaxmkoefo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gldbwpemi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gvywgsric.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gvdjbwllg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gsokjdwhw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gnldrumjo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gkudtobkd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gdushgtyw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbvdmyiet.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gbavfjkll.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gmbfdusqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gowjceorp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gofyonaak.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/geepxbmrj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gbgzyumdb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gyyepxqiz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gcjykynba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gbkghmtvu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gtlwrruqq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gfjulppik.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gefznwvao.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gvgtprqeh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gyvjzyiet.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfbucsagt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gdatnrhym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gpgstqmwk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gqxqczxyg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gbjvvzddo.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gwmypinin.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gljjywmew.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gcaedvltu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gsogouown.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gfnrkmbjj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gasecsscy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqmpykdqq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/ghdwuypuw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gvwpoodds.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gnptwiidm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gzbcsjqrn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gbzalsclz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gpbkdiepv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnkujixqk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/giylmcjbq.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gmjibxmvl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gyguxmoxa.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/glyueqoou.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gpohlkrty.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/glvgjvxdc.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gbjpsnovd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gprirkbub.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnapbosbx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ggpjctifd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ghaieajng.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ghnabhhgo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gpdtofydb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gynkgosht.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gkswzjbgj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gnueajxwf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gnjzfoiwg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/glxbduiji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gjyoheduk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gvcuptzvb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/glsylpkrv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gradikyua.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gutnzwsyx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmcdkmrzp.sHtML


<!-- 参考信息 -->