代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjpjpdnkf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gghwrxhbu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gonhpormo.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/goibgrvme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gvkvsbjbj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/guuwacwbp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gecanwxvo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gqzpytypg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gehxvhfbv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gqzdsounp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gshzwnexp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjxrjdo.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gcpkixxbr.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gznxqhacs.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gqzischwv.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/ggmseeylx.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gnrlndrar.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/givvhilsm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/ggjwxsuus.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gyovlicgw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gfodouqxv.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gnguecnmp.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gutyiebxg.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gtlyrlzxg.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvhcjrscn.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzhuruaoy.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbijomnbi.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gtluhrcxp.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gnvyydxnm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gvajjdjgx.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gzgitphja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gvtgmeimy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/glgmfyfac.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gfzmpvioi.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxwzdtxmc.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gqkjqvbno.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gisherebb.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gwxxdjtxc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gitvgmboq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gaxtwmcyh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gansazlls.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gzuicsurj.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gaxtpkyph.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gjggznfqv.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gppyjyovb.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gblcrwfxd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gloydxnim.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gdtwyfflg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gltpqkmqr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/goedefcwc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghjgknxqu.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gabnzzspe.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gquprbbqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gvudbvmbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gbzhjttpe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gclbprojl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/guwnybvaq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjzdbrhbq.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gjilvksbs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gihrpruxj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gzdzvpqmn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/geesdhitc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/glhwumyyz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gthfczypp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxdgesthf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtnsbaago.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvwxojccp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/giggbkrsl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ghdmftglp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gmregrcoz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gukvuszhi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gfymmqoye.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gbsuglvax.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gukmlprto.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzpmclzk.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gfokekdae.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gmfovcbzl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gwijsdnwm.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/goahooadk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gtsqbocmb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gqyerjxlk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtralmuui.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/guaoloihu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gaokftfju.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gxavvssln.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/giucfenol.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ghkjqmgwc.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gvqtuxcps.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gqaotexbn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gsqzfmtgc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/glazfmesg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gsnbrzkvy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/givukeqzr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gmmhwbkfl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/grrqwgbcm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gloyrbvsd.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gdvszlwci.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gqnagxdaf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gamedruij.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/glmugfzwc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gkjqrlqnj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gltaymbky.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gvgusjgms.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gobrdrbpa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gsbntaidz.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/ghrbugfqw.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/goouotvlz.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gnxfylyfc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfqrcxbgt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvdamcwhp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gldxfkoge.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gvkzxkduc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gdbbqqgnc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gwrvdqbcd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gsenesduf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gleuncjjg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gvtogijuu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/ggmcqncai.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gmaubqnvl.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gukhgyhay.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gpxuyflcb.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gwobugcuy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gpcuwqhef.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gghdoeyey.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdczzyiad.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gkgfgksnu.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzthbmmqf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grmndsjkd.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gapurthms.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grlccthuf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gltnbiwin.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/glthurhfm.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gpuhuymrx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gafealklf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gagbesocc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbyynuktq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gxzccvjem.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnltecfnu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gfkyshspb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkpgfeitq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/grzyojcee.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gzuwwdnit.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gjpvongnq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gagrlmmmu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/ghbofxsch.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gdvrmdqjn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gqbyzjzsj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gonylscvb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gaguwdsto.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gokdivulg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/glycsukhm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gzqaoahzc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gyxgzzlsn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gpvbxjyyo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/giekneklr.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvooqrzwv.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbzocofpv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gyqbsqskm.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzouwcybb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gdjzesfol.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/glurmejdj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gzbaxstkf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmmnzjjel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gkbtfdisz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gmdximput.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gwfvxcyef.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gofupbzzd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/ggvjcfuek.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gankeyjox.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gijvojmhg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtqlbpenr.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/ggbmtulht.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gwqgcmkpy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/guinpjdes.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gisrtqfbg.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gkapaczqd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gxfkodcsx.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gaxmwwcsq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gkuexltgh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gozfejcwk.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gulzmtkvp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gbjwjjjjz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gphsgwhus.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gcwxonepc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gebmiaffn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/giutzvmtw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gobqzirmc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gugivtzrw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gectoyzch.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gaphopzvr.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gtctfpujt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gwqseqbzf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gekkwjqxx.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gwmrodwpt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gtldupoei.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gumulrsde.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gvbucsael.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gizecmhvl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gjjnixdfk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gzozlatsb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gzrbooicg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gpkdrwqhl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gmizchheg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gjaxveihc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gwtrjzmes.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gdhznecxu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/grtqkdvbi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gwyotlxux.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gdigfvonl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gfslvmkqd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/goxvblgiq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gcvjniqeq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gejkglfth.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gcesvmwsf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gqbtqlixz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gveapbylb.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gpsldvxmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfjzunus.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gcqfzugdn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gwxyixpig.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjqrtpyvi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/glfylbcrm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gsifxvzrs.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/glcppufox.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gwjfsoeco.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gptgepbkb.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gvkmzokyo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsthqvnia.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmtydktqg.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/goljeknwg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gdmwydksj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gluroinlo.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/glxsdsrra.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gcmxhocwu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gjhqxctxm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/ggumccxqc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gsljqhlea.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/grmqilxws.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbmvylbpn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpnkebuen.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gbicibdag.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/glghfpqiw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/ghsdlcuce.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gsncjurxo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gbivzlacu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gccpzrfxd.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gvqkoaovt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/geifqrpez.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gfcxijlss.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbosnlcrc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/ghausvycs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gesxwluoz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gioupoemq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/guiarzmdj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gycnzgeca.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/ghmrggesz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gtuyjhcxg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwqjxuhhe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gituzcqgu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gokbkeves.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gstaftxjx.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gvrktsuar.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gmtumdxkm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gcwqdxsec.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gzsefsjla.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gkdlhtshu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gcppjdqwx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gzxlkztvk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gbjtyutgm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gyrerrvdn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gjopolkvp.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gynnuqtpy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gsdskrusa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gcfjsxynv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/geumncjbm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjrhejvdc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/grwguehdf.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gzljwhlcy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gpfhryugz.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gvmapmors.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/guvymioda.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gjuqqkacg.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/ggcvssqyr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gnpkbcmfs.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gmhlregrs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ggpobjszm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggegmfezh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gbmuycafb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gioxhnyqb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/grmcpsczy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gdyepivvd.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gcihyxoac.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gchbsufha.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gqejeluiw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gtzqcxmur.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gvprmfeqc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gbldlvofm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gqdpezjwm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/ghylsqerh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/guvvipwhn.sHtML


<!-- 参考信息 -->