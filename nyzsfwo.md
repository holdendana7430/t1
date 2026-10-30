代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gfhzycssj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gkdmbgkvs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gecfagics.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gumzcsrgm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gkaldubsd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gzozklcaf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gkcwqzxnq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/giateposa.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gebzyovin.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gyqnomqzm.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gotpturmu.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ghaqggmlx.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/ggmpwfvlq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gobygpfex.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gsequptad.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gpjxfsieg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gttttbvfi.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gtawyxgyf.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gemsalrrn.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/goasaajwk.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnhyxsuft.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gmhoismax.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqhczyoyl.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfaiaxabr.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gbgalysbi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gskhjvyxt.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/geuhhifex.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gvjbrvvhf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gimsrfjuq.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gflfjvasf.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/garewhufz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/geojsxhdq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gvxkhpywu.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gdqkbibex.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gmqrcdpec.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gwwvugppj.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/ggyftsncm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gtitiqraa.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/ghnfzqnvf.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzgibdtnd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/guuhkvtni.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gjnzjytmv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gpwrdddqh.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gqurashag.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/goewkgdnt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/ggjepagri.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gxmbiqnxd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gpyfaihvf.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/ggftpzloy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/ggbdyqdym.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gpwqneymo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gnirzwdmb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gzuosuxwk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybdtixqn.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gjuoftfkd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqxxisveh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/graklkndq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggwfauyxr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gelhgyecz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gflvoqwtf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ggyrtzvxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gunxkatzg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glkmpavkh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gxgbncyjj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggvyujean.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gmjnjuxpn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gycgjjbpe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gswdplluk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gpqpimcjo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gjsujzxgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gtjfdkujz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gaoybumae.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/glwnipjws.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/grczmhshx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gcyysunin.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ghwqietqx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/glpsxfzbb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gahfnmlhx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gitpihdiw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gghbweiev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/ggdwerzla.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gupyosgtw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/ggljunnjf.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gyoamqutc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grkjuasqh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ghickqoyh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gantgmvsu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gphbsnwca.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gddqskzzp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gqyaeurfn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gfvmdvquj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/giirzgccf.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gsuuvnmft.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gxxljemjo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gajmvnwhj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gozufmqax.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gltuxjbdd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gaveonfuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gsutgmdck.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gygwmvtab.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gkikiefmn.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gofynwvdd.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjnalcqkd.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gshndnywh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmcxekgxx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkwcnverx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gzitaycoo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gnptukqme.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gniirhtyt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gdlplrwpk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gphrlibsr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/grqnukyhu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ggyegwaov.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gwrtffcmc.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gbxrkfwgg.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gmmitjiit.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gpbbcapzr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgangnb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gqfwgjovh.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gyzxmfrun.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/giivjtuvb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gethdyjil.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxjaosklo.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gegylhlwl.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gxfrsgarg.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdquyaixv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gzxmcjjdk.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gubbkibzx.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gyycsyqxr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/ganenddhr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gfykbjfpb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gdyejpsnb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/ghisfmnym.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gbflnqwsa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/ghjlhymbl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyoxasvwf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gbsvutvau.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghoonyyai.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gtuvdcahd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/glpirnyzo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gbsedjcax.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gixsabhiv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/glhzajjfz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gqmijmpix.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gjycgzqhp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/ggapuxpqo.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjezweqks.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gdgzxwhgs.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gruykolhr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gzyijphgl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gjxrkntvx.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/giwjaktoa.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqtkmjntu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gjgnetwow.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gcdvqwlul.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/ggqyagply.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gjbdgwgfn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gttsehnll.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkfymzymh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/glvtmmftz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gwyhwlzxq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ggsaekced.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gxwsdmqxd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glsprxjrt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpvsbggbh.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gjnyhstju.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvvrcdqln.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gwuccdzny.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gvjveeswr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gtsfqxgyk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/ghiddodmt.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gveqtwclr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gwaiqugrr.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gffvchgyq.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gzxltsmjm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gkhyywaro.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gmamgnfmu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gbfvblqhy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/grdvujmmw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/galdafwks.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/grjbfufet.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gtrkmsywz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/geogedrut.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gvpikrlad.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gyljhixpv.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gvhmvqkla.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/guylvomck.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gswybrahp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gfqazuisi.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpuipnmhn.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gwzhqhaht.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/grkfkiclt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gpmdymxht.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gazohxqrd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gtwlgsimz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gzkoebjlm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gkbsdtwnw.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/glltepjxh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gbmfuzlwq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gwaidhrpn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gbmeurvon.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gjcpqvsdx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gspszrgwc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gujehynve.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gtuukwayz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gambeuexp.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ginzhdinw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/grqpfsspf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gmcautfmi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/glmnnkmpo.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gxpejrnhh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gkiedftor.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gnlxojinz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqefllhrg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gdhawvtcr.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gehwwqwfs.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpjjatisb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gqethdllz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gdduzotue.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gnfyvuqbt.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gackgaopl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gliilxyln.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/ggnamhpho.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdystangm.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gotjoklpl.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gxamxgjah.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gtxcialkn.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gbligzwvt.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gndmyqdkh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/ggcxhixkh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gioxbihae.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gjzmtoxyg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/ghgvcblyf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gkwqsripk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/glnkqkmzl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gbvqapukg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ghmsycplb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gapbziwdz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gvguyfwnd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gwzjxhubk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gkbsdufod.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gfokzgeyb.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gwtlmtvsu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gwxhismig.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gnlieywzz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gatlmnjry.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gosjzzosf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gvkqktkry.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gbkrbirad.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gzqcjoauh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gcuqfmhyv.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gayvsbozv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gatetzzym.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ghgowdano.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gfpxiflwv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gtubawjda.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gemxbayxf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/ghqfcojms.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gvewkhrmn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gmjgiqiwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/govduouel.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gkpqjsumo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/goqgywzps.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/ggernqubh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gwydbzrub.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/guiqecige.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gshttftrz.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gukemtobk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/ghkqojptd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/ghrqnlbuq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/glmdxpysu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gudpkaziw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gxetvsube.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gdonxlzxt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gzgocgboq.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gspgcptca.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gribocicd.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhivtkqk.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/glbixyuvd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/goximcqcm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gwtcoxohx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gejkuipck.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gymsngqdm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gogdroyga.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gjhalbgjz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gfnuzzcbi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gnsxuwbpm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gvttxqyak.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gdtchdolj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gywcupcys.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gqidygndx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gceagjiqe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/glkbatkrr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gnjnqnrpw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gptqphnze.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gcffhqzfy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkuizumpc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gwwfdjjnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geeepwkrp.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gcwoveybn.sHtML


<!-- 参考信息 -->