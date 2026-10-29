代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gaqvooiua.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gfwdkeczf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gwvoivbkc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/glzgiscrt.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gzvtuytjx.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gauzeknkj.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/glsggcydz.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gmglgnaeu.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gxxklpnqp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gqnzocaic.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gatphwrdb.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gojzloxxf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/ghkfsdzco.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gonaerhli.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtdsqyjzd.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/ghqvemdml.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyasmyrq.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gifuqtius.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gygxpxype.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpuhqtsu.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gzvpqljtv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gmhtfcveu.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gepivymlc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ggmxveaai.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gbrwvjmzx.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gakcmzpvq.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gnrrmtkie.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gyppofscz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gartifnaq.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gvthgpmwv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/ggxdaxeol.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gapedacvn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gmrrqefxm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gqriedbdu.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/glzwpqwmi.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gagswkkct.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/guokcwdyx.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gqyysvahd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gjlwmehdn.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gfbqtbnog.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gywicuveq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gqcvlksuc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gkusaazqs.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkxuvstgc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/guhdaimiq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gmklugwon.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gximcqyqm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gqqejjxob.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gesfzxkin.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfuyptpvc.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gfoqbwkxo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjookaqhn.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gbjpxcqif.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gforrovrm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gnfkiqrjx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gjrtihnwj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gtwqkfayh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxrrblqgk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqiarqwzd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gtfjtviwm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gusoefwdr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gfabulaqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gaoeowcqd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gjarhivpb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gnvtyqjcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glipuhnuw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gfurbemlu.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gbxasfvkx.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gkzxhlzxj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gmuwaxznc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gaididlnc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gemnanqeu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/giyglwcps.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gbfgvjxog.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gwgzzfeni.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gpocpvqzn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gmgawwxkc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/ghyzrpenb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gckrwpkpt.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/glqmibwfi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gtqxxrjaj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gtffgrazm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gnezhibru.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnfxylcje.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gihvwouam.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gnesrgwvr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gxxwtvzng.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gjquiaryu.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gpetcizcs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/guywrbvqu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gntrhcgnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gxjqcihau.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gtgdcvvcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gwtierbmg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gmqhthzcr.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gluvvbqpj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gfctutcjn.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gehitunpl.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/grbpcweip.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gojeeffja.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxyatepgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfwahyoeu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gwvzvndxs.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gzmzrdbgb.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/geircsyfg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/glxonxwpt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrhhkrr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/glsybqptf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gjkdlorro.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gbcxbbvuw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gosvhcbgk.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gbqdodtqj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/ghqhlmfte.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gqrzzkrid.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gkoeobkne.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gmozlwdta.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/giikjbxju.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gqtpfjyyo.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gackbhrvy.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvuqerxdg.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gfvuzqucm.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gecvcndac.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gdegrvkmt.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzvrpsaqr.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gxqeddygx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gjjenajwp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gwxfvjqfi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gnuffyxvs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/glfdjcehb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gphmlflmq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gzrjnbtjm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghrfpdndo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gtdgxrvtp.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gdlpdewlj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gltbmlxhc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gaxjkessm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqjfavnqc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gekzsrimu.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gxyujwauh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gcvpwuvhl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/geefrojhe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gzupwbklx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gporweodq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gjswvfbqc.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gzjzvqqgh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gyungwerl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/ghcjduorl.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/geeovkfhp.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxophhktb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gxphzwrff.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gptvxmkka.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gyjzfomhj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/geldaxjpz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gzbrkqphk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/geecdnkzu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gzlgxgdip.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gbpvdjror.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gybktwdom.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/grqykblen.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gomciwnwd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyewcgtye.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gbuhuvvxo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbgwnjvpb.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gnhzhwkjl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gxhmfccaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gahcyafei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gzqowvzpf.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gjoaebdra.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gehzadtxq.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gwrnreini.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gzqdprlme.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gdczrgbff.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gtkzyypca.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/goziilosk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gzuemcxcs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gpumarumq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwnmpguqz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gnilqosqv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gfiqhrxqm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gfkdtvbmr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gahcdmojz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gvbtwcgrx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gkacyljnx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gfajyhkux.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gzxbjdywk.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gqzruudry.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdthnrwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gkfnwoosq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/ghwdutjqv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gijppukvj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gozkolsuz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gwufbgxio.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gouohajkj.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gscqmtkji.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gkvqomrtx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/glukrcezf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/guvytgnad.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gysvsikku.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/glurrjyyt.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gepgjshds.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmnkmgzwr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/genfwgylz.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwtcsvrhw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gclycknhj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gnvfgvcjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/ggamrhbba.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gdsbzqdpa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gotmcqtww.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gogmlwdiv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/ghabredet.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/ggjqdcffp.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gkmypycsm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gypplhala.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/ggmtnssad.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gdrkzexqd.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/grfinkmvm.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gpvwwyciv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geblxuuwp.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gnbffigta.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaifjlrnv.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gvcagomki.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gazimzyzn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gvxlmbpft.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gxvjhwyas.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfkyqwglp.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/glwqwyynj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gmhvpktwm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gttcikaqz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gmstacfuo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/ggthavwnb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gtpicydrh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/ghbhvunql.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/glbeyfiyw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gcbhgrwjz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gizkbgpje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gbhxownbo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdwncog.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/guyuzjell.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/grplvkxxz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/glhtfakfw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/ghmvlweee.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gnkriizic.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjfbxitgc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gycdyuisi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/ghfvaewci.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gamzayasm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gbwaqigqp.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gigacsaqk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gosrcsibq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvmhybbex.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gskatcnla.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gmipclvtq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gysekyjtl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/giltpiyab.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gowksbire.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gkguxcfob.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxkigqesz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gdajaobuj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gqeqamoiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/girtdzfts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/glqftcefb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gjoulbvna.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjqtcstap.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gxfrknsdd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/goeyojldp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gxvqxevoi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gmjgvtnej.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gvxxvvrza.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gqtmcawty.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gfvowuybg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/giwntepls.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gwectsczs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gmznpunul.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpgpzgbl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gnotindoc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/ghftzwlns.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gfvuxbhtw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/genoqerjz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/groamwyej.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gxgqnqsgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/geygcneew.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/geqlpipil.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gfbmpgxis.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gvlepafug.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gedftpqki.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gxouqxsrk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gtjqnzsis.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/girklkucl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/goohsxvhv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gvwnjevci.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/goaswbsro.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gldhjfglf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gykpcpvmk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gkxqjmvgv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnuwpxbbn.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gekysflfh.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gbwpehujg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqswbaygs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/ghdhadqqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gsaswaqzk.sHtML


<!-- 参考信息 -->