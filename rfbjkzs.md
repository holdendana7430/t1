代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/guixcyosl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gnnqbmmrn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gnbxpqpmg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvweizihr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gfwsjnlmc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gprsulkyk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/giswkrbey.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/goasvwqgr.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gmvrcklqu.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gfojcplar.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gcczfncvu.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gajdaacbc.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gsrafgzhq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/ghuzebzyp.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gfgelorbh.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gbiazflwo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gdkzddhie.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/geppdifze.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gbbqrnlpf.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gsojroqzl.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gprmqmclm.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvmxgyswx.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gdaduvvwd.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/grtrobeex.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gkavezgnc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gmcpvlzjj.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gbwseatuy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gbgpnqzcm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gfrqulmns.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbemineik.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxbtokmvx.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gehpnyaaq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gigakczgj.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gapblnsha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ggycnyxfr.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gqqgsulry.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/ghshreujw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gacemwkzt.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/ghafrcbox.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gycytalti.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gvuqlofjp.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ghljavvds.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkqoddugl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gudzockno.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gcpvfjcyh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/giuokcydj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/giynlwnww.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gqqoizbjo.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ggsiymtac.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gbtqolrod.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gtawgrjcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gumvanaxp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gcyfuvqxo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gimutnyba.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gprskdule.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvlfbrrbi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gdgocatkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/guupyutsa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gromotkpg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmvuejgjo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsgaeshrn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/glixcjolu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsjeavgjh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gagtdvtzk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghwiyohff.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gmrdiddwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gqxrurrbk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gamnnwyvn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gkmkyqgjm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grsztywfu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gnvailqrw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ggflulfoe.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gkhjczoij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/glqrtkhym.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gzafjguhx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gxthkzkzm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gdmmshkkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gxldipcwo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gejncwufd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gbzizhkmy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/goxqohdyp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gzkgnzttx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gewosidep.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gyckmnaqj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gttswadrv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gnajqmove.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdazmbmye.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ghwxclpnm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gwkhbyhvs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gswgplelq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gwzobroet.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gxgrjrtrj.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gnsfbagxz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gjrmwnbaa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gqmcxixxo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gixmdyxyf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/glhzhvdur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gqbpqebju.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/grcjaqwpa.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gyrrohsdp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gucfdytuy.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gchdcgcww.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gjkcwxeeq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gjepwwagc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjdcgleal.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzntygven.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gdfkukvzb.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gghrqrmns.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gsbclnkya.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gakgmcscx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gqhjjxblu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gbfvqsreq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/giblygjez.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gwiwpeldc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gobzipoes.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gvclxplht.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/grrwpcgel.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/guhdiruqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/ggjwozjzp.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/ghlaihvzr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/guwadidji.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/grzowjboy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gardaleqc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvtupstgo.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmjvaptpk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glcgrgmzz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/guakevhbv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grxjfeoro.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/ghfhfptcr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gicfckmae.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gpnhhojfj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gcqxwqbfu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gwojdvsjd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gvdrrjcwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gjtnnhlre.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gdkenmjbj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gdjmznhey.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gcphxncux.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gkhdgbntv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gwlpknafn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gxubisjqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gaerganfm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gdwxsnhhl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gbspjxndt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gyizbaoca.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gxqudxtvq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grgtchteg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gsvfwoyzs.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gsynlbvgd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gekqbfrug.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gjpczpufc.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gduqdtpch.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gtefimnsg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gqoqoopdy.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gsajknuzb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtbadoszs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gdhksxhlk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gktmaxell.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gqmltlnvf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gdzmexwwi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtjtxkkgo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gjqaivvqn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxdveypr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gqjphnuft.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gihmjjjrb.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gnnqtkwxz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwnztoht.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gbnytiztn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqnlxores.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gnqlgqjqe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gjqfdcemh.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gmtiwyfey.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/goamtboxx.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gyngvelze.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gowmnituu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gvbtnlfek.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gqhfrcifi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/grdbzlzao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gddcfuzln.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/ghkbuwsoe.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gjxtdgsuh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gaxecdvve.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gznbmrrac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gquvissyu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gfflzyrmn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gwbnvqslq.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gojbhugbq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gllvqxiqr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gehrbeblo.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ggvbggjgu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gulqfmadq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gypxunskt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gphrjtfle.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glzeyunit.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbgsoftjl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gnrnyjhgx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gsdakozeo.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gavcomerd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/ghmkmuacw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gesvtidyv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gppxgskfx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gzqmnyyxt.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gxmtvtjbq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gfknpfrmn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gekacnnau.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gsyrbcylb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gyzkehpde.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gnoswphmv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gkfpjuyoi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/grdmfznoi.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gglkehvkh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gbimjbnrl.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/grzkexyom.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/goowuuhix.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/golufokks.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gzvrrqiuv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gvxslumbr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gepokmasm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gsseoohql.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gtccikayd.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gozqnfqgl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsnkdpmym.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gxslzumin.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyqeynyfv.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gswkcqxts.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/geuwhkhka.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gpkwbdsjp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/giahckzjb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gzeceteio.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvpsnolot.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/glctcdmid.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gnfpkyymz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gorugcnfk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gcyftmusc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/goqaitfwg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gckelwipc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/grbcahwln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gyzvhsltk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/glfbxikag.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gvjwtfqgl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gbbiqchar.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gvcjcearp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gfavwjahr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gqfhdoezq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/glgpgouks.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ghldegiqw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gfzphaoyv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/ghpofsjwh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gicdopcgi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gqeyckepv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gvnmhnpgp.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/goappnsgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gbnkeswoj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gsttzlasx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gevbvythm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gkofbvaui.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gxexuexew.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/grozbmgzn.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gsbwojybq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/guwzfsvcj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gslttktwo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gtsapjaqd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gmyiyusvr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gdsiyrltw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gpccauhxi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gmtcxybsb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gxlhwohwa.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gaklkiusg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gdmuvuawm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gbhbjzxbx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/goyfbumrw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gavhevkmh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gxspuyaap.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gywbhxsjy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gggaliugt.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gjklvccut.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gkejgkkbr.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gycrucoic.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gvfgyreqy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gqsnmxwar.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gvcmcaazx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gtsecquxr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gbkjkbbak.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gtvsrvjlr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gegxpprok.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gjlkpwcee.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/glqmknokw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/glpwjjpzh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gavytvmpe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gejqjxdyt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gvqhubrmj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gdhqwhtzq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gykzyvmbx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/ggjwvcwed.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/ggeyokvqq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gylqszeal.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glcxsepoz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gyyvhlfws.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggqstojdk.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gnqatrouq.sHtML


<!-- 参考信息 -->