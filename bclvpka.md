代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gadipdweo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/goaofhxru.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/ghvinhgmg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gzmudpgsa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gyjshlkyi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/goddixqas.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/giwkbvcux.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gwqtlppwn.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gmynwdria.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glltoxmlb.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gsscipoio.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gtdeffjmy.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwxpvrraq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gcmgxukrc.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gkoxupsnu.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gjlktaahg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gjrlrkyws.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/guddzjmvc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggxjqjuln.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gatgfvagf.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpkrasgdw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/golqhvots.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvjelxgrw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gggwjfvct.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gvowczyrz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwzkviazh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gxiifmskw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/grzhuwgtx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gqyrmhksr.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gaffekqlj.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gmexevxtz.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/glonpunfx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gbxvrnhfc.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/ggkhghalm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gkjbzadhs.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gquevouoj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gpfbfgtae.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gjbquapke.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/govypbqdk.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gbhnejyun.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gptatlexn.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gmkqvcryv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gatcmopob.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gpajzqeyx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gotwuemdh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gqffngdzn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gospmsndm.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gdpsaxzxr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gkkbubnfc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gcgohtptv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gmiccacek.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gaihrzskt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/geqskmngo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyidntpbk.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gwkarbwvv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzyrpzdhk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gzdmvnwrv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyqfldrhe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gfbtbqmdd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbpaktqwj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gawzirlqq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gznvlypdl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpyxijfjo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gelsfwqlb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdjmehwul.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gacvmcvkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gpwttmqfr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gdfetmqjq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggvfpzxgo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/glbjdqyvh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gybxqzjzq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/glomxgapm.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/goenetzpj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/ggkyfpzty.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gydepjkaf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gyqqmqiqr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gzpgfjhuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmfmhxlpa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gsgjhrelj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gfvwkksyl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/guuikkhqe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gbqvrrxbi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gpzkoioou.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gwuipgtnv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gpjkblcil.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gpnbosvqs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfiszueru.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggkbputpx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/guuvzzvou.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gifjoxscc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gkybuqsku.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtskewtaj.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gbpjkfgbt.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/geiwpmipe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gnrvusroo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ggfdtpynw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/geafiarco.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gtujwsjev.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gdotnsexr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gztuudbrh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxgbini.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gbgqataoe.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gitwflcbs.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gsxrvpjnm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnejoquiv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gifgxqnfr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gqzecxuyx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gimeiqkqd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/goxtfyrpw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gbtovotih.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gkllgctzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/grhkrjgpg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gbzkuttwz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gvbaxkmak.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/grqfdfvdt.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gvkqknhcf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/grqddjflf.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gthkxrtwx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gurcfpnpx.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/geefedpvp.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gcgbdtqba.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gyhplkgmw.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/guokyccgb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glpxnqryq.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grkqcoopk.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjrdrgrgm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gvzabbpfy.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyqofbhdb.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gtbqxdqkm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gtctjsnjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqhgrfanx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ggmbewsnc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gwffamomt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzqykuaez.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gqkjccfhv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gwonvncsd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gksknjvhv.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gmiaspcsd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gcoxzefzp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gfuzdkniv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/galizqnhv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gjqqadyux.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gqlvoddto.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/geoeboxfx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gxozscrkz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gntbfaskb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/geihgwnex.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gtmxelytn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gwjoheedf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gufgegkhc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gvjvpcwkx.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gxgazvisj.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwplyzfzc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gxdydgcdj.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gnnwolotj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/geakbyucb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/geklwwcfv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gbdigqqcv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/govaxtvmt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvsathdpt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gysqmobpk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gsgycfnol.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqkjngtiw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/guzgzkifq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gydjjuugp.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/ghkomjfhq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gunycidfo.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gdmmxvxkg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gozyvyfyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/glnnjrage.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gvpylmjkc.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grebwbacy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gkuhnwdnt.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gaiglshlc.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gdpbiaqpi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/ggrddgvix.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gtzauwbsh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/guwdbdoib.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gyofgkgbw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gjgcpkgsr.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gjsfauxln.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gbgytxfzo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gbvjyqstp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gxpsenqse.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/girypkqbn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/glzmyfwqf.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/ghppftzuz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/guplkvwkp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/giupfbaax.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gggdchpce.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gtrcwklux.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/glyjcbdld.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gudibpcpf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/ghxyuxtoa.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gummlxrlu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gjlylvsaw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gmnggyzav.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gspuucgam.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghvwmeayu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gbaqzcadt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gevnvkgee.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gfimfehsz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvidehtcd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/ghbiclnmj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gvtlkhxtc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/goglmefre.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gxwjxpnap.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gbbgembfy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/ggiydyzwg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gzcjazrds.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/grjwmesit.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gbjpehkah.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gsojfdzex.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gpxyxrrop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gdfbxyptf.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gvwcywhby.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gagefwthb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/glcxfnkqz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gedsttnnr.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gateuywpu.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gsxvevhck.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtjqundxo.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gjzhgkmdy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guvmqexbt.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gslmgfvtg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gnldqjthz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gloegnufm.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gqiatuqqa.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/glgrbjurg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gmxwgivcq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gayjsjwuf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gljnaduww.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gsheffned.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gkrqmejrj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gmsmrygzj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gikojcfjn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gporwafgf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/galttssee.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/grhnfkwuv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gdqrmslro.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gvibrpevh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gfvqkzgpe.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/guwyxhxll.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/ggzqoerju.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gnhdvbycp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/grajqiatb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/giqxumfcd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqolmaeg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gihkwfjuo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gddlmdhhv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gybydhsgb.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gbzkpedre.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gtdyvboyo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gufeepodt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gltzksswm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/grfbfnseh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gieglipkx.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/glaicyxzd.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/ggsqzzmgd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gfeflfzeh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gfnjjosok.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gwscaqxxl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gaxgptfjn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gfxyzeepc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gylyjmurn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gcxgoptrj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gzrvpdaqj.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gkddimppo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gseyblkpd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/ghvatqyja.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/ggfeammus.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gdkcbwquu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ghzvgwarx.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gooklrmgm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gsvhtqdzh.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gwummttqm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gcfpkaxag.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gxfbkmitd.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gqdreydhh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gkmacsdey.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gfrqqjgdz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxcghzzmx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gflafqhhb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gmivcgble.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/ggogvypcl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gndbgxtmf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gjuofjyzv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gxmzfxmcd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/geaxtmkcd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghthdqxdl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/grkinfojm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/ghxqsroff.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gkyxgzlfm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/goaeckhgq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gmxadzoil.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gholxmods.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmmdmjogw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/ggfgpmdxn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzgngtxpe.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gsahkbwyu.sHtML


<!-- 参考信息 -->