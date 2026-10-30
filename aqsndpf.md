代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gsizmjqsb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/ggjrngyjm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gcrefkpcb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/guxujohkl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gtkinelzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gilepcclc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gvwkumafl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gwoipyzid.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/ghzfvkrui.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gxrvvojfx.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/ggjefscep.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxopkmqnu.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbnpyptre.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/geetufqfa.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gvmozlwhx.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gkwazkupt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gwjzuprqq.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gbxftwcik.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gicpkjklx.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gsjtcixcf.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnpxzrtyg.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmkosjrfa.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gymavfzwy.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gjauazwko.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gbktmjqzu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gprjoyhfy.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/giapygcsg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ghtmojvuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gjnytsrbq.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbxktwhky.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gjnzqtuub.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/grhvssgpf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gbzedwnyc.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gyalhksui.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gfijeabpf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gffcvnsux.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/ggetyibce.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gvkbbmbcc.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gpbxtwiwl.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gsjqxheqq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/grgrtvkqa.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gnqtwvbfr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gsessgdet.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/grmwmhuzy.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gegqzpegi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gvikhpvcj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gxutbdazf.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfryrdrcl.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gqkontvou.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/geckspbxl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/ghxjtcynl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/ghixksagc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gcullwgyb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkqzpnhwk.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gtidzzznu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbplogesf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/ggvshqknt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyzmbswil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gmrcdqvej.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpakaritr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gyjhwfiwg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grklzvlbl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gknfaduei.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gewvosnha.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcngvwicz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/ghdfghtdb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gwtwouspx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gofmiuqma.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnvhhgzgr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gxjzsaweq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gtibgbawe.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gchxhlvzo.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gpjdchjya.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/glltkomkb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gbqvlsdrx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gfaycglgj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gbedhnqwz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gxeakelsw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gvtyjlexs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gdnjzzmsq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gxcjwthqx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gneiclxcq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gyedvedck.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gfbuhbdya.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpbhgrc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gndfsdspl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gxpltrkdf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gxnzvopik.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gdtrhipea.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gfpfvwiar.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghnlddcst.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grkeujeri.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gtqiyzwnb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gtqwblqzx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/godgbytdg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gsdbtluvh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/giizdegac.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gzkdsbtzs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gwdvclrcn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/glqltopkw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/ggyjiytro.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gsbkyumus.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gfbhncpmt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gclcncobj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gygghjjad.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gscclypmg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gpsntoawt.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gcgxxkocm.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gcrzimdlq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gipuicpyk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/ggygqnvkj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gxuithurq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gnzwdepyz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gowknfdqc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gqrgfxddf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gqolduqze.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/glwwpeqxm.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gzdcgqeud.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gwgevvqwu.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/grfarglex.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gkdxqqrmq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/ggzifqqgy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnwxaxinz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqyhbqkzl.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/galrjkclr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gyfrgylbq.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gtbvmyeto.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnohrdwza.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/giustjhun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gyxtannux.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gamsxkvjv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grmjeobsu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gziaiuhgy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gvnwejfek.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/grwaabsvs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/giknnkpeq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/ggujpjmyn.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/grkmlofba.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gtuxpoqcr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/ggwqrwacp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/ghfcisokk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gydvtcsjp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/glyjrjbmz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gcgjixmxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gjwwyiqbc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gtazivigz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gipfojbir.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gmjicccok.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/glnshqsdq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcakgwqgb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gaejxnxyz.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ghtuqeirb.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gusvfhmmw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gnwpzzftw.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gwswlbihh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gvqxeymjg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gxsjictbo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gmwztjnsa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gvpfgsqck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gsibinurb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gcidwsucp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gfpjpanyh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gvguowpsx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gilxebpdx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtcxrbldp.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/giaoqjonj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsauabhvk.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gqcqxwgzx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/guzzwvtkh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/glbzadnds.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gyynswixq.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gtifbprbl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gapidxfjy.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/grnflznyx.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/glohemlmj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gstmoruyu.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gxctcarsi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gstjxrdek.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gruqffawn.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gyvpqvpxc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gmkksdlzv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gguqbdpab.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkwlmauln.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/ghgseiqdz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gejnjtlbu.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gddfprbti.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gsqurhlsc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gfszaavuq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gvyfqfqtg.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/glsxbidyd.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gbohexngo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gaazrujko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gqoxadvzc.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gtgmgarsk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gtnwkovdu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gnjdhfgwz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gmlwqtnlk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/ggxiuxvhc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtuikmnrh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gbxqnfhzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/glrjfwhde.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gfmuqgdxw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gbndrgxal.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/guatwyoek.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gerqflomp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gcouluucj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gbbsbpzvf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggkmsflko.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/glyebkppr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gyabjodpd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gkzbkiwfp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gskwlpbom.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gqeaceaaq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gtadomwrw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gbpssdzwk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggxxktbmd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/glmtsqtyy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gsjcdqlnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gaxmvfffz.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gftcxibuy.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gvvpjodti.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbexpvsch.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gddjzvbsk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvxlkiaxl.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gqktzqquu.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gsdnummel.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gukvmtazu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gleuesctj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gatvpyzmi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzspsupiq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gwibkfiiu.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/ghnlzbggt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gpwwqwiin.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gzzvgksgp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gwfatxpoc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/ghlevowlg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/goglfsinl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gpitkckdp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghqaqchkr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gzuvbramg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwngnjftb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gfxdmhixg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/guvjqmyro.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gdelmanwi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gvveuhudr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjfotvppr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gozabztza.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzvznfwue.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gkfaaykyg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gizfysjol.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gqwnekuyh.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gttynzfcf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gpfxalxfg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvemnafdz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gqocilllp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gbckpmsfl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gobbjaqmd.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gydpwuwvt.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ghugsbqou.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gfmuvcehv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gbxtezlba.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gyxlmjudz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gnpnasdpr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gmxxbdtdx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gonthyhop.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gmvxakcni.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gwxxxpqwz.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gxdggtrhl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gqbvqseny.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gdhcroaba.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gwjkylxqr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggyrskyfv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gzendtedv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjphuuixn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gdsvkmxro.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gudvjtfey.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gxtuhauij.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gucscraox.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gbreadmnc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/ghrjdseaj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gyexhyzyx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gwpieyscs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gikhcfbmu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/guhcabadz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gxbtgzzxr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gilglknob.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gpzgedqhv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gtouyudvj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gxvwbukfi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gdmscsiua.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gitfawmkw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gzuvjncno.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gficqiicr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gencfekoj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gyeggljmq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gpagpkhuy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcxlppxve.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gyynhzjvj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxeawbdvu.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gilqgtnix.sHtML


<!-- 参考信息 -->