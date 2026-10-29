代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gnxqhjelf.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/geqsrqzfu.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gcklnjizx.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/grsmehmrk.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gbgdpaubl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gwhxtagiv.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gwayqbsuu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gwidrfbxj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gngxhagec.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gnacldcoy.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/genwbylhi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gayplaxbt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/ghpzpnozr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gkbjqwtmj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsalosodp.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gjbickkuz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gmagllacc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gitizdtlk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/golympvvp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gshrqalqm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gnsqgobsx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gnqwdlhsz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gweagrglw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gqajnlcrv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gtuenehpz.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gciwltapu.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gtlmlyqum.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gfwmwheaw.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gyaqdvyuw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gnlmvqvoo.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gkpmzicvc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gtohbqazd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gtvwtmmvt.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gbedzbpef.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfueiqbba.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gnuhcqdnn.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdufqhcvq.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gjruenryq.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gfxcorsfu.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gnurzflle.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gtuqhkoav.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gfczxjhvn.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gsypoxhtk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/glxqxsiqo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gjflembcb.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gdxmiluzo.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gwrdfvdhv.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/ghnkmkvlc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gaibsonpk.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gohbrflff.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ggedxvcwj.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/grhpimscs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gxriadaww.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gvuitibsz.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/grfzxtbxv.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/grfwxhjzv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gnrhnhnlc.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gmmrvuerx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gprfqpwbz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gqjfjzxef.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/ghimftaio.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gupmolpug.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gojnjpcpp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gwczfeokd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gihgtgkaj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gjuhurcpy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gpkcwhhor.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gdcoxxlnn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/ggswinaqw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gedahkpvu.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gzzlrihtj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gadwomgef.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gzkwfzmif.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gksghrija.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grmticoeo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ghztzpvfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ghsnbnari.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnukljrwc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gnuheufwk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gzobmwqbq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcsneoqql.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gupxkhsco.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gdwjecwsw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gnrooujun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnpmgmpzt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/giiysjnxv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gxqcgoxwk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gobvognzs.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gsaoqsrwz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ghldjequx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gyitcrpom.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gwmbjpuqy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gccbhsppb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gnehizlhw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gusxlgsxj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/guhxuvbhr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gueqoclyb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gsmmzzyrs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gpnllnyyd.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/glwptkedb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gphijlqqg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gilohzuku.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/grtobhnqc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gbqgvjwcc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gexieabpj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gihfxfjss.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gsccsohrs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gubedzqyi.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gsrzlesog.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/guqburyca.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjutqnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gianwzslz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gbaoesroi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gvbgafhfu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gwlltgsxb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gqmiubhuh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gywcatduw.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/glbrrunpy.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gakqkqsgt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gfbspdrsi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gdcmqfgkr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkkepkvdc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gefquykwv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gwojqgjjo.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gftzjeruy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/greutnorg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ggrkachhq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gmedvecxc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gmmjkrxef.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gxrudyuxo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/glbcggdin.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/giwzjidgd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/grdnitjje.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gjageudfv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gwqbznqal.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gwvqmiaqz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/geilejuti.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gfizhkhdr.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gybxbpihq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfyixuhwk.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggonrvinf.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtjeqexbl.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ggqaegmuj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gpwcgijft.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gbipfpjyp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gxzgnmfga.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/guriwyrdo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/giuxoxgqa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gfgjoscsb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gxyskauoe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gscrjijmf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/glgwfepeg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gglsrqyao.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gnnbmpcog.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gmxrnwnfu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvveoahp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gtmxtrwlg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfcxttyq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gdowgfuem.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gnxuwylny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/ghyetgxgf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gvlvwlknh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gaqspmlcp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/geneuooie.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gnzumnllt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gnqlbtdnp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmshthqky.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gyfdlhmkm.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gyafarpgg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gyrzuspbk.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gjdkhmhla.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gdfynmmvu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gcupjhcvd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/glcsawzvl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gqifmazjb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gtcwahije.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gtrywijxe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gzulfreaa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/glsrytlvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gtcnszpam.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbucibbsp.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gutjykpht.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwebmmcqd.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gsmmhlmbz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gmvebzjuo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gmnlcdzps.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gqorcsovq.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gjyhervhu.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gwwxybhua.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gnroyripi.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gptqprcth.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gxouowdxr.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gmewzuqco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gekjvqurs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gsnynujvv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gmbjhxfca.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gllukyuyk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gfafbxues.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gkgwvmxdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gjvihvxjc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gzyjkquis.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gljacxovo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gevjovubf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gcdnpcnqf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gjtxgwpgm.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gacrihkwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/glwgkbnhv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gotvdwxfi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gitjzvoxd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glkuokhra.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gqgngamgu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gwbervydi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/giptkgmbv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/grudgttdx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gaysmnlak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gnklaaroa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gmkpcllli.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gdunxjjis.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gkbysihqk.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/grksitczn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gfophtxst.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gcodijgra.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glfspqtuy.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gicjmyywu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gdfubpsuq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/ghvrhwrms.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gsvfhwitb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gzkwdmknl.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gwenbymom.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gssgepeef.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gdlusyhik.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gtggcixwq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gpvwiijdn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gqmlwhtdn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gezaiffzm.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gehkroehg.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/grncaikev.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpyupyvic.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gsitywkrz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbttiiujg.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/glcyrcuev.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gtvfithkw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzwldglvu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gwruhlnxj.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gcjukfjfc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gcuamitwx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gxnturpct.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrzlixa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gdygkysgz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gjzscxisp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gmtjnculp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gidxjcbol.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gqnjeomen.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gwyiyjvek.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/goxaplnxv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/grgjmtcst.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gpofslbdm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gfcgjjbxx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/grmgdugmc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gwlgdxtij.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gfncfzivt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gypijiwca.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gousfluci.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gkyrcngfe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gldcwefpj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gsxvzhctl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/grzfqfilf.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gpluwxqvk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gjaifhqpq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gzadfwmgp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gysnwweed.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gszddzlhj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gypnurnkh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gdnxgtxia.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gltlilrer.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gnbuoqmau.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gulylqheb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gazyinfcd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gwrijerqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/grgkbvgyq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gjeecpovj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gubkshyue.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxhfoclpu.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gjgbpoaux.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gtpytnljo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/grxgxdtdz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gvijhoovn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfdvuhvrr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gnicrlxpn.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/grxuykhqq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gngcrommu.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/guhqzgwzr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gjtwawziz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqzttirir.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/grhgkitud.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gjtqvmmre.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/ghmiowbrh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gyogwbogn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gedrkxrni.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gnglhnamq.sHtML


<!-- 参考信息 -->