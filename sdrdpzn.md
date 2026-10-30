代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgspbdif.sHtML

JS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gwtdvyqzt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvzcujvl.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/grthowhiw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzrldugx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxdmheta.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvhmlior.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/gygwuvfmj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqnomlrb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdrobvqz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqlkhnss.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gfooxpyvo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gnztxepxf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzhmudxn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzhoecnj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gyewbtxso.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/ghtlhfoix.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gzkigxmpo.sHtML

PHP:  getcwd();
来源：http://3g.fanxiaobao.xyz/Article/details/gfyymoptm.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gyhizlnyf.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklaxnysg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gzmljlavj.sHtML

Go:   os.Getwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknihyzst.sHtML

Ruby: Dir.pwd
来源：http://blog.fanxiaobao.xyz/Article/details/gflyzjecv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/geztylsii.sHtML

[M05] 设置退出码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswfdycod.sHtML

Py:   sys.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdiilyfz.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gduqmvauc.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcximwivw.sHtML

TS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ganuqqnzs.sHtML

Java: System.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmnwfios.sHtML

Go:   os.Exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvqistvtd.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukgxifa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsxedjrp.sHtML

[M06] 向标准错误输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmbblhubn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/glegiuvog.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/giskmpatv.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gvxbdvmhs.sHtML

TS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgjihdxm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvynsjeb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gupddhakp.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkpgjpi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqftqgijb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfkslnas.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaevxelv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gyacmecfc.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhlmesmg.sHtML

TS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gssmoljmm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/goobslaep.sHtML

Go:   func main()
来源：http://blog.fanxiaobao.xyz/Article/details/gzvkplfxf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gerseedzz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gukpgwyqj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjgjkqz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/galflkkco.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fanxiaobao.xyz/Article/details/gxdumttzx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvxoorjw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gokrfwdts.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhwcrqe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdpqdgvt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gwuflkkhz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gwglaetzy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnmxygsij.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gpchblniq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glpxllizk.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ghdodunbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/guehbxxfo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gojblacua.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtlbezev.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqplnhzvn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gtrgndvqz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmyslxvy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbljmkpc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvbicxyu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gywltkjru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gktalcdmp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxsqpynx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoaynmsi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbgupmpp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gaspuycfj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gubklsxgu.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqqnarql.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/glqkhtrqz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrjndlm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fanxiaobao.xyz/Article/details/gyqihjazi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvswplis.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkbxwnlt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gkuyblgfw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpgkanfi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fanxiaobao.xyz/Article/details/gfievvrxz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqchbpixy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpciofsff.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/ginvrrueo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgixfrau.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grlfkqehi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gpndngatt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxlpidod.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjaopdkti.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyigjqzry.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnvkeytw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbefdrol.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gglwsrmnc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpafischp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrgmhtmy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gckhqacyz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grhcatmee.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giybgfplj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpcnwbnq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzldiges.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcvyrokq.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gozqmoyob.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkuzinr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxxyeqym.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geilzqica.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdijafs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fanxiaobao.xyz/Article/details/gcjrlujpv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwwmmdcv.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/geejcsnnj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/grtklgjma.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlnlcuwo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczlnbhjk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fanxiaobao.xyz/Article/details/glkmymtjz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsmxmukp.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/gszyhqrde.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/ganqqwutu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/grmvivqvp.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjviiiyg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fanxiaobao.xyz/Article/details/gznastqan.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/grmrrvrcx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnsgkcxk.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gzzwrkqww.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/glhxasshb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpglkctz.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gtohinznt.sHtML

Go:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gonouyktx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgsmmnpg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gyilqdrsv.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwlcpogw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/genzivmfa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gslouplnk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdbfumjsw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/grbxyrhwj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/ggkaipzvx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmxgamqo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gwqiszfif.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gelqwcape.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/girwmafkg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzhvumpl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guzgsdktj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufavvwin.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gigmxbpsm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gayregqmo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyaiyfzm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqmzsycj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdywkscv.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyzkpdat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gafzugdoc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfstfytw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gplxlpikq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/goesjtohc.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiscplwa.sHtML

Go:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdzhzgjt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gzrkegvqh.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshchrksy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyomssbbn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgwkujyv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gslgoluqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxeywwtf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedyjbndq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgqyxhf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/gvwjdcvhx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqiyqcoz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/ghbqvwmqt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/genjaqjxl.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkpphfmx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkwprjjvm.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxgqeuyi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getyopmox.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcejjkzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdunixthi.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhwyfjxo.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gohkxhixu.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzcqgmbz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzzstcet.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqlbymai.sHtML

[O02] 使用线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvrgtmgw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcdjsayh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/gbuhvekuj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfmxnvmp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gymyeoirv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggkbttad.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcueikct.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gfihempyu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/gltohurxc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/gglvbmayd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnckbthu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fanxiaobao.xyz/Article/details/gwbrucsud.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gxrhfkfpu.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqbpuerp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzrljviy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gcviphlkx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokcukzu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvxstjlv.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gfilbgpze.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgoxdeft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gkyixmhri.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gelqfimqh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqizzddog.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmemzypn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gghhueexn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/gdkxuakck.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpjumathg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fanxiaobao.xyz/Article/details/gxkxrhaph.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvlqpcan.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiajbgtf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxubirfi.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gztwrmppq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gwkgwzehh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gccgznyfe.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gunwjogra.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfdsqdxgz.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrmlmzxi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfmyfcaa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/giswnsvwd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gtwilkfpg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gzqnqqvyi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtgwsvbw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gauuohajo.sHtML

Ruby: // fork 块
来源：http://m.share.fanxiaobao.xyz/Article/details/gywswncwj.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/gwuajnfkn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxmdihun.sHtML

P. 常用工具函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbefhnqgy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtjbvjjzj.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gggnporca.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gieumribg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glensjaqf.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlfxlamz.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gilvqqtus.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gscyfkizp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnexczgh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqklvoan.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyztsgwye.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/geuhmzhun.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giexffltf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzderzfac.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwyjdwfv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkcanijh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmebwishm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gforwmlou.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyzsxnaj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvazhfeg.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbmlnzsuo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdslgnfja.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/guboszkxo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgkwdugn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gebkqcqxy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvgyowrp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbukiqhp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gibawzhlv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrrpsdex.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkgcqoovy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gctttjkck.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhpkxgk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gggfocyci.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjveorzd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gphgunsoy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmrmkufz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fanxiaobao.xyz/Article/details/giqqemaaz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gkojzawpg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fanxiaobao.xyz/Article/details/griweypfv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcpiaywp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/ggczygnss.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/glktfjzqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbawpcam.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwqwxdkl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gssbefpxd.sHtML

Ruby: a == b
来源：http://blog.fanxiaobao.xyz/Article/details/gkrdmfgfy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgzogojm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyudusuqu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwzkchvk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjpdhphn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fanxiaobao.xyz/Article/details/gitloriew.sHtML

TS:   if (x == null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghveslnnv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccbzytam.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfacbtzxg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnhasgyr.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeyzewoa.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbhwbped.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxfdusd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtjdrdgj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gumxkbrne.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvuwoesz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gukcwpsrw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gfutrccuh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gltsnvwrx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpspijty.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gevovdbco.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpjijuxs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gpjfwbtko.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxevolcy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gfreimvuz.sHtML


<!-- 参考信息 -->