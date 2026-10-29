代发 wailian999

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gzhpgfzpo.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/guoauhpvd.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gqgoisnil.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/ghwfeebtd.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gpwjmqcwc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/ggjjjjjqk.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gcsjhhmfd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gnosiojuq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/grmcyowji.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gyvvyxxkw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grtzgdgxo.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gfcclpuss.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpddzmgqf.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxbkbxlzr.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gopzprcnr.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gxoedaghr.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gjqbaepwp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gcfrnyvlh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gyabmbbeh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gqhxxkqhf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gvfvssikj.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gfuhymyth.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gdfpucjek.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gwtnjirzn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gqvbipzba.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/ggmcusphd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/ggbdwqcjs.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gnxpizkno.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/glcjsoleq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gpvqgrqwl.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ggjccswmx.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gjgrebtht.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gxwqjjtap.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gkbykgbpj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gptxdaugg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gcmtlcgjr.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gxujtetse.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/ggqoefyfd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gpznuqwtc.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxopjvtob.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gsrantxwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gergpecam.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gohmcofle.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gdvdlgeui.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gshnjjblr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzuqvyuyr.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/ghzlchzax.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gypdppvxj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gouyoxdft.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvpgxqefo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gammztahn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/grjnexurj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcaacmghj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzhvkeuae.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gycrjdtbq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/ggtgcvpoo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpstwiccu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gdzrzjegd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtvtjisqz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gspilnend.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ghhrdxszd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gamlfmvca.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gaqlsuerw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gyskxldjz.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gqmzgwirt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/ghfogivjr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gasbnloru.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gxiawriqu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gbylhzvwr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gycwodgwq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gaoehatrb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gysrkkciz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gvcztsjum.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gbbmvzatf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gvelcgpbs.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gjgqssyms.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gqsanwdmx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gkucotacb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gnglbajpu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjfshswgj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/glpsqosph.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gwiakdaxc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjnufxyem.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gljuvfmcv.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gfyjwindj.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gedhvrxyz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdzxfqavv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/grixsiuln.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gsoaeqduj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gzfxaxlfn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gvplejosv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvizbinv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/guybbblxo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtwoswylo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gkrukfsxb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gghyjuwfh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/giviwtfxk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggbwdpzep.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gwvxfjggg.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gmvypbfww.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gtyqtbmhj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gixmynfyt.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gharcjtve.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gskrkkcvq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gqypyoujm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gqomwddft.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gmnkicarl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gfhagbnps.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gcjdjzxki.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gtwmwqpdw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ghtflpnyc.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gofxzxuda.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guhnilcgo.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gsxgfeeco.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyyczhaxb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvefiyydd.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gylyjkciy.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gnalbaxsb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gdgpdzsch.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glnxpuxjm.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gkcoasvob.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gzhonyjdt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxqwnnkni.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gamerxhgc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gxyzxfnmc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/ggmvqfgap.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gdlnpofun.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/godiwncdo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gzfzsjjmo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gqpygkixr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdayygd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gavhwolzz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/giakwxlyz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gtkxarrun.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gbzlgplso.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/grmkzwvww.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gdsdddbwi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/ggtdjdyqq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gfydgivcv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gjczjmblk.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gdodvdrpf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwknesbox.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gpxrnkhau.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzkwvgkpk.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gwotorbrp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gztmoxdtv.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/getyoxoce.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/geoyiepml.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gynacdwbc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gdgrkwpjb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gyafvfsfi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gnuqpbenb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gvxtnijgg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gpranfhka.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gxbybtvze.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gkewfmpeh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnlkszlvq.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gnyyusmcc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbhidaarj.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gcokpintw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gmwibyiqw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdurrsjrw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gpubcvxgt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxysbgovk.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gjydwmdic.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/ggrlsatuk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gnnvpeiyl.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gzyfujulx.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gqvfkjonr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gpfijemal.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/glggxehal.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gfamqvdmw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gubczpdcu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gwhzpyaxp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gfjydwxhw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gnvqpgzae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gkgpryrgw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/govoakrve.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/ghpzhcvoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/grueoodam.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gbsjeyylv.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gkrgqmpdy.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/grzsnqcvc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gjlthtlch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gbdycyujf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gumnbjqvf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gxmvxpxur.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gkrzdlght.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gjpvaputl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvezshrcn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/glzrufzel.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gcrlvxlvw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gwpmphxxj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gfnhieowi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gaepltgvv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gwpwhpyoe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gsjaywtzl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gvxblibjm.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gkfmszrye.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gysasyqbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ggwkeecti.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gpgmgwuus.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ggrngjdxj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gcfhbnrgv.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gjfqsaqjx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/grezuzncz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gxuvbosyz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gnewufgyj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/guvjaiifk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gvhghvgtq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gzkodvioy.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gpcoajgfs.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gfeldpwox.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gazkehquj.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gnumexvqb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grlulsktg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gmtoxfdxl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gdmzqgkrm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gpklvsykw.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gyizzzikl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gpypnunpt.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gaabhfbtz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbkqdknek.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gmfwapewh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gjsvmvrrk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/ghadsgbbr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gryhoqidi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gdvaomaqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gxgumwwwb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gmzcrhtrx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gsppncexo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gvehyvlsd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gydrxmvyk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gbdqeirxl.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/guofpuuhn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/glauhfoft.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gzwibbcbh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gpexgkhhg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grybiqkls.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gtxcbcymx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/ghdckdqmp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gjnzgsagj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gztooqecg.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gvlqzbzbr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gqlmeaslx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbcgurecr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gntlxpxqg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gtdhvijxx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gcbhryxlj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gsrwyolxo.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gjuuygyfd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gwvwrbxuk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gtenzdlkb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gfpdpvfbq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gxfgzjqhi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gqeuenmok.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gceulwtwq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gnqsvhbeq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqhmycshd.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gehddtflz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gldmzrnfm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gcnxjwfvp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/getztsdqu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gybasipte.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gmjzdlsmq.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gjhlrzlnu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gbzycsscv.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gtaliofge.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gjnchkmrp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtvwsuggo.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gfkwhshxb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/ggwfoxvqr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gmqrajeqx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gfcudkdqi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ghosesirh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gxxgnjbbl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gfycwbods.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gfuapgjmv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gvhtbvoqv.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gchlajdrd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gkbnrgvku.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/goqnfpyxj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gzoowixzq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gafdjtbij.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gejearuan.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gudjuyyed.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gzjryihfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gnjbxfxgr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guceysmtp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gimxalijs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggouzhrmm.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/ghnofmzmu.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/grkrfccob.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gomqvthfs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ghrimvygh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gewevahxn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gnzeyslka.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/geyxrtinv.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/guhqsuvew.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gzmlkittf.sHtML


<!-- 参考信息 -->