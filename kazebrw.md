代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gqvsrkyiv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/glplgzvuh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gfahqeatz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gajholhcy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gfrgctjxi.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gjqfvnhgh.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gcsezwomn.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gghbjgcbl.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gradihgkt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gtzulqhpn.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gzlptadxr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gvitmwqwc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gxdlztlaw.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/ghmqezzcp.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gotzmeaey.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gkgfkyrdq.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbpbvomnl.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gyuqfqdcm.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkukytfoy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/giiuylgka.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gordwfkhq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gixlbnayg.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gqxmfmxbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gewvytlms.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gezprradb.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjysdxxky.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gyxesaupa.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gdrfygvxj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gicfkuycb.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gcmemcycd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/ggjqwlskm.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gioqbmxff.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gqcacqhbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gscmnadsv.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gpgzigrvq.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjjfgzbau.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gdnrcwdim.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gemsthydb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gnmoksfpt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gwdpoqiuy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gdpnuplnn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gzppnhwom.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gbryduppo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gxkvuszea.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzllaoktf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlpxuqoj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gmqcjvihu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gvsdwozbd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gwfnpvxxw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grffhsgrh.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gkuiyjhco.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmapzvfe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gdouqldgc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggqvqcakh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gfsidvtpj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzdohebrt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gjifihwnt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gueiqdzhu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvnpgziun.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/grgtvorqo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxvjgtxne.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gswbpinvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gefdauobz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gnzlccufd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gmvlfxuik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtmymdvlw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gzagsayhd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gsxwrjeju.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvjqncsrg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gvtsjrhtq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gczcurpza.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gnmunxhny.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/griikqvmw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gllknkguy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gdaoaiahs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gmorrvuxa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gxmlasihp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gyduvbgan.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gvxrznctf.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gylntafda.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqrnsqflr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gaqvhhcmw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gpntmzyvk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxdxxovod.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gskapxmgi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gzqbbyuvm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gqadqnlzf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gcvotwayb.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gczykmyav.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwscqcrdz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwodvltnc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gyhtvvgia.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gpkbqopur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gfefqzgho.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gywjewxms.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gehhfgtof.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/govccdotk.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gziyviyso.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gkfawcohm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gyqqbboca.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnexscgpr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjwezsdtv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gjtgjgcqe.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gzzymqrqe.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gtmuteruv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gbjnfuxxf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gsqrkbssm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gluaugmdg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/giabmepbz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/ggfnknvrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gtnuqvwnk.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gdkuxcjjl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gtapwunxx.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gsajgjqhj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/ggzqoziug.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/ggplntjae.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gygqodbpf.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gstslnxlp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/geaytrwyj.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gakuorczb.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gmjuhqnwg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gagtrauoy.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gmpsgvyjz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqxdssujj.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gfpqkmfff.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gaadljqdw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gqpkaqzhf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfdysyxxy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gvvrzuxdy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gomwvbfqk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ghhaeeswr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ghyhlgjyl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/guozulgey.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/giilavlsr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gxsucmvxi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gxyvmvvrh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gdfaqphqe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/geiqgreik.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gavjcijpt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gackgoxfe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gxdimkllz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gzgclhdtj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gtevvchda.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gddnyjnna.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gkbjzlofo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gswddpyat.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gogocqrnj.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gyujxqfkf.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/goyutnoyl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gumawdzma.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gxuubbkma.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gbbeliuaq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gisnewhkw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gurbwqvpp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gsknpwfzy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gunjrgtck.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gkqhtifxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gnxvrocqy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/glbhrqmar.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtslubkcs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtmsvbkxo.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gerawbddz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggaqzielo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtungwe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gpogqxqxr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/geveqskfm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/ghhszyjit.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gizfbsurd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gyfljpckz.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gqoxxiixo.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gxhmmnbks.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gjgmfiady.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gimwonjwc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gtomlsixw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gnfboaami.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gqbbutsgk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gajaydjyc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gsbtcahsv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/geazybhax.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gzvmbfkmk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gofucstas.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gfxtoxoty.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/ghxoatkdk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gqiaojvxc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/ghavgjojf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzyuueaxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gggfmbdtc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/ggwdeocar.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/goazijitz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gzpgrgwbl.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gbyiwsqmr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/geisuohoa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gydzxvame.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/geboeqigv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/giedlaumt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gjtuhfkyw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gaxlrehcu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gewsaypwj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gdechybru.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gdrabmdcr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/galytxhdu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gefsiyzqv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gvdmslofg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gkvcmreaw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gylndcntj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/grasfhbbk.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gavsrfrzi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/ggrktnoyj.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/ghdcxsmtb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gdjzvzpvz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gbyjayley.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gxezmjndq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ghnubttsb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjcszvgjq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gkutohkey.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gascptxpr.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gopesdfdg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbwmyfczz.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gnqlbbxwf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geszcfiga.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gwzcciesv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gepppejge.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/giutsbdjs.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/ghalshyoz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gjkrqzsxd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/grekzqymz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gbsavsdqi.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gnkcaacyo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gdqykmdcy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/geqftvwhf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gbrrjwhah.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/ggqxdjxyc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gssuxeabv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gcatmwrvx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjrjxvzhr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gcfgsawhg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gnssrrcpv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gdrcjizwx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkcsxhtcu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gzyfqhzui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gzzylyuby.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gfotxebyc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gnxylpvej.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/glstesqzm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gtsktyqzj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/ggksekzzs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/ghmffjwfe.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/glawjvmda.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/ggmzynita.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gaaiuybdw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grdrgexkl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdfauhxoh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gqlsrnvar.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gkzzxecrx.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gdirrcwua.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gdinsfmfh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gcksvdgmk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gvqcepbbf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/ghzlkexrv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gjnfxhlzi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gwpgkdgzy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gphijuzzg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/glqskxexv.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gvdctuoha.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gynrrtyxp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/glfyhvmej.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gcvafiuqv.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gwolrjyts.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gnqgzxrby.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/grvrenygs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtghfnjwx.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gumfqcmzc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/glqzmksef.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/grtfywmqh.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gshmghbcr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/goahahqyg.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/guzwuoxuz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvivfpdcj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gsdxqxrls.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/galzvqrts.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gwaulmszo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gfvehjwgr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gafspidvr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gsjspuyzx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gjjqhkbim.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gunhhecro.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/grmdkevbc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gcfdkowpo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gxjedhbnn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gzshvcoel.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gsdsxrfop.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gycdjhvfl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gooemctwf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/ghwujulsz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggukugmku.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gfogpkbhg.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gcewytrph.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gfsrmeziv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghzehdnxo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gnsfxrrhf.sHtML


<!-- 参考信息 -->