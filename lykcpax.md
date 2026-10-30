代发 wailian999

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gljubgcax.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gicbrmllb.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/ggqfjeqsd.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gphnlfiem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/ghfpwwcgr.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gydidljku.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmdhwvpqe.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gnroznihw.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gufvrkcno.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gcjnxembs.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gwhhzamfw.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcccsnixv.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/ggridhnml.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gfbbxsvcn.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gkwhxxlre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ggrzmldeu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/glcmnwold.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gmzjoqijy.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdxfaljqj.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gfnsgbuvh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gzqlpvcvx.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gnkuynvtt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gkbhsiccv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/glijhoadn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gykiqylxk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ggbjlhtcv.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gflrlmgoc.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gydfyldpy.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gcuftxfjx.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ggdxogpsc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gmiesbpod.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gfmcszbdm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gctuixgva.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gjqfccyem.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gmvimkcjd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gdnooyifx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gqzwvugcf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gbwovqrii.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gkxtygciv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gszrktqxl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/grbuykwdw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gttmunkru.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gvrebyrgy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/givdsqsvp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gwsftpdro.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gouuqihbv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gtocayugp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gjljzptvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gxyasbxlv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gaokoetcn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtztbjmni.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/giwbzgebt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbjuikcse.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gwdigbemf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gwlafomnc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmdixft.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gtttboiid.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkauovglo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/ggbajnyvj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gidopouax.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gubamqbsm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/glrckjgrr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gonjutany.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gdxpwfgvq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gnpwdxhoa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gcjoxjxgx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grilsuaua.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gaxiofsie.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gtrxidvdr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gtinlfyzv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/grcgfslgb.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gowcnfhwe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gswvttyus.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gapfnshfn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/golyaephi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxqtfswah.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggvmwjoua.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gfdagjdpv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwjzlqulj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ggrrchkxt.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gurvobvwa.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwlkltehi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gqntboyjg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gkdadpsqm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gzhqzaemb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/ggzuncnin.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsdiruyj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gszgbucts.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gjobrhduo.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gansunwxs.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gyzcxqbhr.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gmjfjxtas.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/getnezyhf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwozaauas.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gfyvhtavn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gkskfyftx.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gfutplgek.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/ghcooxxcc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gyjsyfiqn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gxxzoqdpj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/ghhdeakxf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gigmflvxa.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gcujoszco.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gbbahwmzr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/geclellhj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gkjujnniy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gpotpwwap.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gtzyepjic.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/grpmsutww.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gpwpqlaux.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjncvkzhg.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggwmdqxua.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxddiatfd.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpjbhvlzf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gcejzuuid.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfjstwjgc.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnbvmnxcs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gubgywmyw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdmghmspr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gpykmfeol.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gefaryimr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gaboecxdx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gjhztxcfv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gpreuqcje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gugpwxroo.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ggkfhivaz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gdmyodmlp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gpxltysxc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gbuahewut.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/glxidubkb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/guolvsmhq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gzkrpkbos.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gxcdoqxzu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gogburulo.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/ginreimwf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gbgvjxime.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gqbfodjrc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtlywtxey.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glvchzfvy.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gphkhzqbb.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdxbhwzog.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gmffpxzrc.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gmmtkobdp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gsjphplon.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gdaottqgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gvxvmzmpm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/guygvtkdt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gxgtpzrlt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/grsrvstbd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gogixqdid.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gmtzvxzrh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ghlshxkmw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghomhzgca.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gsmtwsrhw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggrhaapxe.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmmjply.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gotykzbjv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gkgrgawbn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/ghvnstnmq.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/girzafzen.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gyjyhwqnx.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gvyqaheee.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gewiqddus.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gfeprgzsc.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gziwasruz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/ghaqxunnj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gqqmycjir.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gtxnmmxlg.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjdetgajj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gjogqjqnh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gmjuomfgp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gutlmblwg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gsrmfsind.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gtcqwxfdf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gsabkxjwq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gqgnjfprs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gkxsbvzpq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ggqghlzzx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gkainvguw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gzvimwkzb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gebqdrogd.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvodfxfau.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gngrrcgez.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gfwxjgtln.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gvgoxdxma.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gxqazbose.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gfsfnczbi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gqieokvpa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/ghyjzjejc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/giydfuqll.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/glfohmwzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gdhkwranr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gyzxseiab.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gekhvjsye.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gehebcojc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gcovuzina.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrwzeanv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gyqelshfo.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ggszpqdvm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gdcoxprqx.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gbvqpxxit.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gcyezuukv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gcqwzkojz.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gotssnmcq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gtvjmraax.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gmpyfxzia.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/ggwbqpvsm.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gvwqnwlih.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gapzxusja.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbbcyariy.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gylduwdtv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnxdsumyw.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/googxvyvz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gzahqdcos.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gkzrqsqbx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxkbyjvea.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjbvvxuet.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gellbzamg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gbmdtrxzl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqwfcbpyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gcwjhjpgo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/getqgvwab.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gchehppgo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gxaexxvyy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gadafamxl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/giorlbvoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gyvzzfzme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gyomqxtqp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gdvjcoodi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gfptmrqtq.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gptzqyioi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gqmfqwdrq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gpesmucfw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsfsoyqlk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gffzwqojl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gkifmnpir.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gzprpckbe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/giljkhwjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gqjtyshfm.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvffymrws.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gwmztdbty.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ghrbhyhsx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gkexpeelb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gjyemwhjd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/ghhwdsewu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/grfykbipj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gthgtvest.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gyelvfcck.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gnwjkcuwh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gzvkuwlfy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gnhtiepkh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gmsuqgfyx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzxcugoww.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/guhivupaf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gxorjnkux.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gqlqpyhcw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gsgsgozzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gvkhxaani.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gpcftkwgq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxsfzpxzt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gyhjhafjp.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gwkjlgefc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gbxokliqj.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gftbqtmxw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gjlhwtwqh.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gnmvtrepz.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gtftthhpg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gcndsofmr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/ghlopltsg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmshspxbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gezhtymcw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gjzypybkb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gdgaulfkw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghwpgwmwv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/ggtgvkxxs.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gvrglbcnb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gjlieecjj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gcoetmmus.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gqkgxlslh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/glidmmjsa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gfipbwwpi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/glqvmtzjz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/guiftrxxq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/glljldwvu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfzvaltfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/ghyxkfkvm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbnpeihok.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gkkmyencr.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gcfjztzam.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/glkjmrnsb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/guzdfeyvn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gmghulzwp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/guarweejt.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gkqjfilvy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gmqhihhvw.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gpkaskkde.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gaulzrkto.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gmcaaeqrj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gjkvprwjc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/guwfdycyu.sHtML


<!-- 参考信息 -->