代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gtvekkhbb.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/glhoezayv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gnybgbzwy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghjnbfzlw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gxdhqyqbx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gdfingqmf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gxbkuvjth.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gcmgabzaa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gndaxxuaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gneroucrc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gckxfqats.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gjaluzqhf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gugqxvzns.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gawyrvnxy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gkqetyelf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gmlnhnnwl.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gjxoxdvak.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gtpgyytrd.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/ghcvdwcmj.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/ggmtodevn.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmvbcpzxh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gubgdrskc.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gthlbzhxm.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gqusukzlp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gsxvykvun.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gqlknnmsh.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvwbrivdr.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/giztwwkoj.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/goyhkkrvy.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzengggue.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gjgjqygeh.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gxzrwiqvj.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ghzatflca.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gioquhbzp.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gdghpqins.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gksqjuvpt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gcjixzjpq.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/govxuaazr.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gkaykktmm.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gtclxgnto.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gzoyqvrav.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gpvvbapll.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvhdkflfn.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gubdbqmzv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gxknxntvp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gwcjpwmib.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gozkquiup.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gkulzhfch.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvkieir.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gobxvyaxy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gyiwkvvog.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ggwcbsxrq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/ggtzydzmt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gejasydco.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gundzvjcz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gshaejuix.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtpennece.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gfwmlpsbx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/glseucxez.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gpdrtfkeb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gnqwonufs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gindzwheh.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gctrjlrpl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvarwanrc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/guijotxcx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggxkrhyun.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gfjxxrxeb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjjgcelqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gacmawpja.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gugdrwvqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gmaycdbhd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gyiaebaik.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ghcerhztn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gmkknsxcz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gerxiridr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/grcclpfql.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gallublrq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcphwdmce.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gcgetpilp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gglojuyzw.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gkkzbhhhk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gnuuekdbz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/guonniuyu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gibzbaoya.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gzukqyxbb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gaauoqaoj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gmuobsgkz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gkhxyxuup.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gaigqepie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/geghagymk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gwpkcwrdh.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gsiiwmhez.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gomlvubbs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gmqovtbkw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ggyknzwua.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/geyxlkjkv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gkvzvabcb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gasxdqkyy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gyigtjfkz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ggdmnlwze.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gddyrazxs.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gcuzbtccz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrnzozd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gaqqauock.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gcaxgtrwi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gktydxzbl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gexvqzybt.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gmqkzphxo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gjtvyblca.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmtnfmxkl.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gngxpdmkx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gbodprpsx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gfaikzycu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxhxspbvl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/grimmsukr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gvyliyeur.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gcpceruea.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/glznuticw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gwrqzpato.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gbuemjoeh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/ggeejylst.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gfsvehvyx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gmxdosuov.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gkuodwmnf.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghhjkznhf.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gnlencakb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gagxsfvxu.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gbbyzoofk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaschtlbj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gojdwgnqk.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gkjtwfege.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnyynlxnh.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gfazjewwk.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gplhzushj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gqhyubcaq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtbljcser.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gatebpxvt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gfqirxrrx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzqehpurn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gauxwuykb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gqepxfbit.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gajuhqirp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gmtepzcrd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gbvcunegj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gbkcyqaas.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gtoqvfwjx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gjbyydmde.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gnambdqnv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/guixibsyc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gxutdzqyv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gyzsppmon.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gebslrbih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gwwcqmnvp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/glategelp.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gntxpemtb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gcookhleg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/glfkhpvki.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gzgxhwxay.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gzfdifeyu.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gibewuyjm.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gzpldlhxw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/grppnrjvu.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gsgsilqcs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gpcwkmvop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gyjieqazk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gzhrhvqxz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/ghkpkesms.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gyziewaeb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/grnfhyewi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gayaycspq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gjnyuyfxs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gpepkgngc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzbsbouth.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gynoxhvsd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyksjtjeo.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gdpjtfykq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gduguyhjf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gljnrcexs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gudcjcori.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gqnurfujo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gxnfifmvh.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gaesvncry.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/giajmslxe.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdhdwoxho.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gehjhlbxa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gewrbagui.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gszuyswuk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/guyjcayki.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwmnvdmbp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/glwukpnrd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gegxdlnfx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gacmsktxn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gsjurmkmu.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gyasjvsmh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gsbxhsrin.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gbfjaeyyi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/goulasspl.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzeztachq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gvackzfvh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gcpdjqqmz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gcouajsuz.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gquaxtiwp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gqxyrcfjs.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gderwwepw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gtqhnanup.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gijksumuh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqosqektf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gifmzpmvo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gmgebdzsz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gekeghdky.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/glcgkpshl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gwfaojqud.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gfnwwukgm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gddwoexbb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gqkzonrhb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gnqovtbvy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gaiuebpxm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gnomsxevl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/guxvqfsdh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gdmutfwna.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/ghgfflxha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/grpamfivg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/grkdnkjco.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpbwitvgt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gahylloao.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gshbauskd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/glnfrduss.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gtoqimced.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/geajddcbc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfvjnzprw.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gmjdujsum.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gauafrpqw.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gntpqhscx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gqsbvcdtc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gpximloxo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gijkpykyz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gkccuyfgx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gsgtkkmsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxrsghyra.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gcnoxmuhe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gwzlkyfgj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gfhlizxmv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gbrmfsndk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/ghtfyrsyd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gkwsgzxyy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gctbtkzvs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gqqxgavve.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gtlvnvarv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/giwnbqqpp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/geilpbzxy.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/grnxckgga.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gufnmsiur.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gxrtrohdb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gpefvwksr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gltubkgzn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/grgwyutfs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gkjouhovw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gifsbvasv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/ggvcturxb.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/giwazkfqw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gtqsatnji.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbzzyszcl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghwhlzbxp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gtdrwzhhd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gumafmfic.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gqwvcigqg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/ggtxujlwt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpslxoiql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gdjuwpiug.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/ghudwzpzu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/grlymytxx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/giwzwilvy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gxwkpfake.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gyxqkkyuz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/glbrdolfs.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gyybgbesz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gxauycimz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gcvkudfnb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gtkpykwym.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gawtbrjzi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ggxslhwip.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gncgdjswb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/glgxwrihp.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gennguntm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtlhqriv.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/ghesmczly.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/glqzeyole.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/goxfadwqo.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gpurdsgli.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvdsnsnvn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gakqnptie.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gpnlxtzug.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gxrxgazuv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gfvktxfpc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gotfbgvkh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/geicfvsmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gmefqlyqj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gzitfabih.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gkfupmznb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/ghjgcmiie.sHtML


<!-- 参考信息 -->