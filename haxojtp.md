代发 wailian999

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gfjcvbdej.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gpcmnaljl.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gcyeufflm.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gausmaxuc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gqcctwvyq.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gajtjaazu.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbraitrzi.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gkpvzqcna.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsddmigto.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/geafrufba.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gngldbcpu.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/glkjtmeji.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gmlfjuiqa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/ghyapvdzo.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gxnbvguoi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gpowbwomf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gztmwlkca.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gdoecxhkp.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gwubmamic.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gbrfeqxfx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gpdfdhuey.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gchfgtsey.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gquatuqrd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gbkvbzmft.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gsjmdkvbx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/guuozesxi.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gbehqtfgf.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gmjiqvpcq.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gnxmdipdp.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gzanokwyt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gpvhenwwj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gyvyhzgfi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gaociqdpr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gsumnyetk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gsqummavm.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gzywkcnqv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzdgcnkws.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gyyjfgzpw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/geglgikzd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gpqevqsta.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gqgwzbiwb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggtzxmrdn.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gldtdcgoq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmchthvfk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gvgjceslr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzepqfgos.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gxzzcpfww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gfbtbktzu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gjvorufdn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grpgitkms.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpdwyqrak.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/glqpsudlu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghgtcmxsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gmpxbesjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gnrbxxpcu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gylhjacbx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnpwbkmlq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gplxepoaz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gljqpdoea.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqzzmikui.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gpgxeuefz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ghfkazrif.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gymryavys.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gwexlwhjl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gldhjanch.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbdbrtdsv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gcqbgaxhv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gijimmunv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gztrrmhho.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/ggrubfydn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gylelpxya.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gftkeccqf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gjzygenqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gzwlnvzxv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gluihkspm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbavlrjfw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gnunptysy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gitobetyd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmycuygpz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdswxqvyo.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gkbakqfoh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gxspdoppj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gkrmztswz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gcbkbjqdf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gefmrlhjc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gfyxszdvr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gfxbxwpkf.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/glduwddat.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/giokioqjn.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gphgukefy.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gugzriwbo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gfhipgewx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gjjpkygxq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmhavblei.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gqcilkonc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gjnewdqcq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfooausbk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gdfmqbmej.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gomaiwiyo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gvycmlvzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gcbelhcfe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gotskcpxh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gsjypmmmj.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gpgnkqwsm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gxiqfakwr.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/garycqfah.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gtsktkuuq.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gyxhaumea.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwyweqejp.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gjkkegscp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfzwatnqz.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvempjdop.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glrgdlgcj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmgburmhl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gmyojafwe.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtdhrnfnh.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gjysdmmqt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpkzzjhlz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gkexfaocg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmhgwoioj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gighzfjct.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gzqntisni.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gikbndhgu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gwpnjcoob.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gwrcztafe.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gbyeehigc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gcccowxom.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gacbkaywn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/goohcbqpr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gsjzmtnko.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gbtuvtaam.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gqygnghko.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gwtmdhbmu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzrxywjg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gkltzvqgs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gdvmvjkpz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gsgavpzjl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/grjknyxyz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gyqdjpmky.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/geajylpek.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gmdxswkre.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gvypiscvv.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gyfdhrith.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gvbgimwur.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gjqfwakgj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/ggwdukoqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gxdzibudk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gedefaofg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ghjaprkmw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gdwevypto.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gublihanq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gclmdaork.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glpkgfevx.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gfkzrowsw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwkuzcumu.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/grhoszqxn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gxolyzmut.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gshjkwgao.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/ghwrhkpdr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gzkwnqgls.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gzlebmcok.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gajadlesf.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gveyryscu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gwkclvifd.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gtlklgije.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gfnzxdfjf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gxtwirotd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/galtekauq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gxznplnin.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gwbbrgbrq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gomuoruwr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gysizerye.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtjlkdl.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/ghrvbcwxf.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gbcmigmjw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gpzyzraut.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gcthrxwvp.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gglfxfciy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gspfwrwex.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/goxcdysfm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/ghhnuzmsl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gbcmeazht.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gvusorflw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gpczozeze.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/glpidhvcl.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gybiispcy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gxlivstgv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gmbnplmbv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gzytrjjiw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/grikqdwqb.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/ghentsvrl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gppgiclcx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/ggnvzimjb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gjcfijmxu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gkigtkbkt.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gnrspsjtl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gzrdxxasv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gyxuplugz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/goqxybpab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gzpynrotd.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gkgwccici.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gtobmrtsv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gggbcwcej.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/glnpudqfh.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gkpvqgtce.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gcwkdtbts.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gitphwrcv.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gurtyjtht.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/glchpaarm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjxsxkrjm.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gnqtlheis.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyahlwbqh.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gnmlbckjl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gskpsyqnq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gyqkmqsim.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gjgvqsyph.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gphgiuvqo.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gxpvxvnpm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gdwntmmch.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gewnwawpz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/ggpsyclyu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/ggjsprfxa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gdatzevsb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gmxvzygbj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gnryfxglr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gvaenqnng.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtsqsmxwr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gjrmfotdv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gxgvecezr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gmjvetexc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gkeevfuvw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gfnhxeksm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gaoukugos.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gioojoomv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gtrlndfyl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/grqcnyovu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gqbxklkye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/ghsdqjose.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gcbmlhnrm.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/grwpmumza.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/ggtldncek.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjtpajqsb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gflfaprnw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gkiuneaek.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gsskisubo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gniedznlv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gbptaunlm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gtfnzucag.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/ggxqgehbm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gphtwqqve.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gvwscaqbn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gldgryicd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/goyyjxkmn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gqrickidn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjyqlscfq.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gcajjdykd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gnxurdjyv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gtwffcgni.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gjrkmxbap.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gzouotxok.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gqqjahipy.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gijybldsl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmswchjva.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/ggmpzimjd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/govsiojan.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gasypvxko.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gqjfhdeap.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/guzueaizw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gitsokjly.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfpxtccvh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gffuwxuxc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gqhattjii.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gnixrehqb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gdapygwpz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gauqpymal.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/grfpccibk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gnfrutkup.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gwqinvzls.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gjzxyoyof.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gyoyspydh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gbdwtzbgc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gedyezube.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gxxupsohi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gpasapemi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwvsaewax.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gvbvgzpjk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnjijrihq.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gxjbjgdrw.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gsqgsersd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gwhtykjox.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/ggbondokp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gjdrtflnk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/ggvygrlyc.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gkvdlpgve.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gbpojprld.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gesswbymd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gnthivcmr.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjbvxxkuq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/geqewkhkq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gopcpyxdm.sHtML


<!-- 参考信息 -->