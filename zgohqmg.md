代发 wailian999

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gxmjwnkqg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gcvlxdmwl.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gddmgfdit.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/ggrirwkos.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gvteebmke.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gxjchjjsa.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghaqzawfs.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gnzeghreb.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gecneowlu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpeldvgdg.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/glgjejoqc.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/glpcbuddx.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ggqtwkhvm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gbvxnankl.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gjmaepbto.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gybnxhvgz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gusamyaai.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gclgidnlu.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdrdfmeii.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfwhvfdf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/ggvnyujym.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/ghkamkzfg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/ghldqigjy.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gpafhfeqq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gicoisolp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gvcahzczc.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gpvdwkfsc.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gcxnejkes.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gpxrlbncx.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gmrvgqbas.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gbtvimeej.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/ginxkoirg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/goxxrklat.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gngrztezz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/ggvhlkapg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/grmdzajyt.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gmiopftjy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gmdywcrvj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/ghesdmihq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gipczdwcs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gdmtcrjjm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggfdbqjlu.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gwcqqhjxo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdskdikxe.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gdkivkcon.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmajpuslc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbgchqonc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gumcaiezm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gdcklgzpi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjddiyqcy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gusgpbzbm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gybelladl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gchsccybr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gkwkvlgoc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ghiixdfkp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/glryipsir.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfbkaxqgp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gavpvzuhv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gombugkha.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gjkaalcbs.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gbqtjndco.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gqeofvams.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gaktnyutq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gxdicxrpc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gphyuucsy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gwqbwwmrw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gmixlirre.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gbvoztqfa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gwtffnwyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gwjlogfxc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gidrjvevs.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gjsnserjj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gyceawzuw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glyrhgfce.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gtojwiamk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/givesndlw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqxjqqeml.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gljqgnenv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gzgyhhtts.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gdxjpgnqi.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gbdmwspff.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkhqsvklb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtjhhvpro.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gggjatscg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gpkxgnstm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/galbdqwbo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gkcwkpcad.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/goybkeeue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gjtqymyfd.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/guxtwzjel.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gprppoyhn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gemrfyzhm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gatyhvnsz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gjpderwzr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gvjjtafec.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/geamvqbkl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmwoynhhu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gzkktvwll.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ghbqnpxuj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/glzfwiwou.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gozmknbze.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gvmdykjpq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gxicazwcz.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gkrcdahmx.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gocivxmni.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gywyqcywa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gjpagwjpw.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gzrekacne.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gziuxwlos.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/ggyjvkwof.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfyaswpby.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdiopzvwj.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/goxtiyhpr.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqkjoitfa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gacdrmujq.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxpqpgecl.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gugpkrzqz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gtqoibbvl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gllhkukho.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gjilhfnmt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gyjbdyxvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gptzreniy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gxtpkyjms.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gdpcgyhtf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/grngdcmbb.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/geizbzsku.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gytizmsov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/ggebcoodr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/goeoccmxd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gdjsihgpo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwujfqnu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gptmxmbar.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gpniwpafj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gvehzqzee.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/grrqdnacw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/glymwczib.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gzamvexgl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gqgtpewwd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gvaqdwzys.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gwgnyeoms.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gpvlyhlnw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/glhtlwoft.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grhimjhzu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/glrknmoqg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gtiodcjrd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/golsfebir.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gupiohlgj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gyjxkdwui.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gajrbnviq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gkcupbnyi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gozdecwbo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gvuiskqdz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnixblozp.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gojkzmumg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjqimbswc.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gqaexumtv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gcgnscoga.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/giiopmkhr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gynqzkipf.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gtxrctqgt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/glemerald.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gwycvjvjo.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/goaqksbyy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gismkeuci.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gmplsgrlt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gazkkygdm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gponudvzd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/ggcopxivv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gsyuayfdj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gkssdvshg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gawhpoxcr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gswvjptak.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gtcokhfxp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gxgfsvceo.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gwiruxyyt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gajtrfwit.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gabdxdowt.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gukctoqmi.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gttihdusd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gslfserkq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gnqsbptna.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gdddmwucy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gpzldfcih.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gifbninpc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gprwedtoe.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gshqskckj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gzocxthkv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gqfznxoph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gsluubsxw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gejwqqhpz.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gsjxmeryy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/giudjkbpi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gadshdqrh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gurivytxq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gpvqkebji.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/giuugiyhz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gnzzdphin.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gajeyzogu.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gjkcylnix.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcfuyvlo.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gtwzmgmin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gwnifrtxx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gggnfodsl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gccbovqbc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gnswdkdre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/giodcpmpc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gzvvrmbnc.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/goopdpjni.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gmolkaphk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grixetloy.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gdozpqogf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcwhteuoa.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/ghfavcafn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/giefxgdym.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gqvbklnao.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gororejbd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gdhdicqsa.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/ghnavuqsv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gfcmoprlh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gorpeeboh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/giwxqehdv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gsbbeypei.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gizjrmxxf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gtuqechqp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gyjhyccue.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gdsevcbic.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gvupljwac.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gottidwfr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gthvtiqom.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gysdxkudx.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/ggxxjjbrd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gzfnhiemt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gwelqiuid.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/glueiyonq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gpnyknxyv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gzqbzxtmo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gbtimfncz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gjqzoscrt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gnbvjpaxn.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gnpvzssot.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gsiazrxul.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gssebxlsb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gfdnjtdwa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvwzztalg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/genbxjaou.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/guhkdfauz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gkhfrhygn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gjitmokra.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/ghtpnfrou.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gdmzpbnmh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gorjypkrm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/ggtuojlxv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkmuqdeim.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/goxynuutx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/goozqfjrq.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/guvcbzhel.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gzsoiucrz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gfiptznqp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gmgdsvmjp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfjsllgld.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gwqrjhiok.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gxvbnmkab.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gmwmsegif.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/ganeftfxi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gbtsitpyl.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gtcncmpqn.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/glghlxdhy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gdkqsscrz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gxzsmmsdv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gpbgexmmm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gdvdgpuml.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gskjvgszf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gvkjpbkrt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/golydkqmb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gcnfjhboj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/glhjfmrzr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/grsperzfv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gfqqdgzyb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gzviyktup.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/ggocfdvgj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gpofkwymi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/glcsnlzzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gzdrfbhcb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gaozrxqfh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqsjbhkev.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gttzafwaa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwkknhrol.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gtgsnmssb.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gyhpeztyk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gahzfukho.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gcoxbmfnf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gaudwcfep.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/ginmovfqv.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gyryjhkgt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gcuoydesb.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ghpmbpsvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/grlfpxghn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/grpcgyleh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gqcfudyve.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gmsrjisob.sHtML


<!-- 参考信息 -->