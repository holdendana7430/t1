代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gbjcxhxjf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gbnxrddvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/guxmqkutv.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gttdkiatx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gfsgcvhls.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gmzwrgttt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbiwpflnp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gyurkqgdn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gucwbwulh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/ghscnlvso.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/geozeohvl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gzvqxnljc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvcmkie.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gxvqmqhdn.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/ggtgdmjqy.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gjqmwvatk.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gajtiinil.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/glhyfrggw.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gyzrbzpoj.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gotyzswtb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlvxvzl.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gxuiichlw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxrawqssj.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/grpipogmq.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/guggpoxkw.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwpowyevm.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghtdlvpki.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/geybdgnls.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gpifeeppu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/goyehomsa.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gpiairtli.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gwlwyqdlf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gdvwjgjye.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/grizndlhi.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/guhlnlbwk.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gzcerithb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gupyncnan.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/geereqolb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/guqmfntcw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gljjdsfiy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gwixoqnxx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gyvnhttpo.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gnxoacjfb.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gnhxxotzm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gqvosbgdc.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gpupiwvib.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gsdxisrch.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/grkbfgoud.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gftyqqcix.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ghwbfvjre.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gmtoshnea.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gzbaixvaf.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gpqbfsmyz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gtlswzkiv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gecemjcss.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/giaesctyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxpenqavn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqxjyjuei.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gaypuwowf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gajlpniqe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbhkmus.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcxgohdyo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gctkdoumj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvjuwgodn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gjtedpmix.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfkclvrqf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrutiswe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gmoicnwqp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glcdhhpmj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/ghwhomtbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gejyltoft.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gujhsxlhx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gzcrgdonl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gxcenywjg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gtbomdepm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gnsmzxyvu.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gzemdzxmu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gweepsenz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gozwkyrky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gusozynmz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/ggroccnqu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvaemoitr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gsfzdfoef.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gaqarrmdy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gggrtjupy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gqkulwmra.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gekaxzpyz.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gwnklnmxx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghfmjeqjr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/grydeuowl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gzbiziipe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gcnqrcwnm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gfqytgdex.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gfmybkcms.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwkonqawx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gylrktpdc.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/glgglilas.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnqecyuuf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjhlilswp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gefmgsusi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gysvugfxv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gfwdwrikk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gbpqgawnw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gspxmgpca.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gfqydmfrh.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/giugmejzu.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gkbxaftki.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gptrugmpu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guxjhydyl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggwswshdb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gtruydpvb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gjlgcghbx.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gljgfjdpe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gziyjqqzb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gdehvplhz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gjzxibysg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gjbomdnda.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gzrokfsyb.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gegtsnwnq.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gamcxeilj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/glmdypbze.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gyvnyhmux.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gksdcrerq.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gffrcvyti.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gaoihvolz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gujkgsudx.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwchnflya.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqqlqjkpq.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjabibbvu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/guhkvqxru.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gahvakdud.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpkpmxtwc.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gikwbxymf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gcakwjsjh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gtbpojxej.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gejyylqfm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gajkfahsb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gcwgtsbve.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/ggndypwcu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcdcdrjrr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gwfijotxw.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/girwnabyn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gabdvvhce.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndetitjl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gabemfjpm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gsqwlaewu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gmzgxmbes.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gguvpphbd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/ghacyklvo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gzfponskb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gyhejcwqp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gfxjkjskj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/geulgggjv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gllnbkzgb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gxsswxtmc.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gagbhqrrq.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gbetzhgze.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gusnfwrub.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gnvexxbxv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxoyxwbah.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gaifmlmsy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gyimovjqc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gunobentl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gtnfvemng.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gjxsucrrm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gukdxmcoa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gfifrngbq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gazskesxu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gocrfnwhq.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/givhjlxkw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghdpruqkv.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/guyozgybp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gjjfibeys.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gpvbxfhso.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gippgvnbo.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/guqcqgrpa.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gsevydsyo.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/glwdejosj.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gxvnhgfek.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gfnnnasct.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gfdixptxh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/grweflaff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gjajhjprh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/glqarmevp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gypfartzs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/grjagkbju.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gucozgurq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/grxpvmwbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gkjhdpslt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gynivvrxv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/glxauqfiq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gukokjssc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gjtjdfkqg.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gkndkledz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gayvroxyv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gmeaugbmr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/geregbtvp.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/giuofzesy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gkfmcsfso.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gchzckuky.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gsuiwnzcu.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/grkueruuy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gfzxgrghj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gtskblpgu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gegpjwwdy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gnyuxjriw.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gwqthcxsd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gvqjaxbst.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gghmmwozx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gmmzebuwi.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gbrstxvok.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ggkontjkx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gzysmvrag.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gxyioloko.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gntnuwnub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gwtfowykb.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gkivhjwla.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gioycvarz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gfrhqoeff.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ghcyphxui.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gxanuqldo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/grewgnemj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gpcjmvuuj.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gkggdnmsn.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gnnriptfo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gookilndd.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gdoyvayvn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvfxetoey.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gsnylzesf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gcfhsmagr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gggpbuupm.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxelptilz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzczumpar.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gomybnebu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gosuppjkt.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/grshxuryd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/grqzbnaxr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gysfxhaql.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gzdxvnsvd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/ggkrxvntd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gihxuulcr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/grwocuiog.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gnhdruxsf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gwmoalfav.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gxabqivkl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gokredeci.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gkhrcpmms.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gkpyucgsk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gbmswzony.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gitjaohhu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gxzendtpf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gxmzcsxpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gjjudpuvu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/glngutqwc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/ggcyqfpnn.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/grshcdlwp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gahejabvi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gacuzpbzc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gdismtpfc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gtgngknce.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/glmppyhcn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gsredwkjt.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gshstbtka.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gevctyaxk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gwwyzptuh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gcvgszkik.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gksszfnbs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gaogxfcyv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gcorylets.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gijczmjxn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gevmttmrc.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gyhcrleba.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gxpkwadfi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gkqmusews.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gtiwjpkbe.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gyfdhsvpe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gmlluxpvp.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gizkfkuwu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gafamwfgs.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gkulykgvo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gxtphrdfe.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gqgoikjco.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gmpinhgwp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gnbmemftd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/guynumtbk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gmrcgeqyl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gydcnlcqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gfzjwozlb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gorebnvrp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gjnciqcoj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gqrjghzzd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gyvxofwae.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gaiilyowv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaaaevxaw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gxrzfrswf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gkxfcaolc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gftnfogey.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gwifcktph.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gxzzydwjr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/goavfchyl.sHtML


<!-- 参考信息 -->