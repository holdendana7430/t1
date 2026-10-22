代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jicaocru.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cilpylkb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbvyimou.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cowqkgsl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2chhciiqv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fynvtilh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hgzknkhx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ibusmbld.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rjmncsdw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vurioppv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lrllswcl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yhxhbiof.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2akprndgc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cfzhluez.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hjcmjxne.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zdcsachj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2izghcike.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lkwcdrcp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oewfzqfp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jutpbsbt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cgzzmcrp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gfzerbvp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcjhclf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lumayhdd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cplljvdb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2eqgtwysy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hspkjqbh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmyxzxc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sxiarsly.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vjzynmoi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iltedmhy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ivkvsxxd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wblyjlxj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fvqfuhfs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uhiprkhd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ftamrpvi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cybzbzex.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gfvufbmc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yurququi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lhcqprzk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kpahckhc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vbhqoonw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lcznpalm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tenliged.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zhogddjv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sghwvmuz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fjsvgkqu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cskjgecz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tobkxltd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vuvtxsqv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vxkzlxpr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ajhrxsdc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2oivtoaft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jllialjv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ifarzifn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsgjikgz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ssjehgij.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jryewbxe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kooqtyha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2plxysudn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qdkdhrig.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lzhlromz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gblwqovq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wblumumh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzduqyqu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xogmddml.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eiassiyd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kecmnjhk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bmlkxkst.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bbbaeexj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bpwcxwqe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bplfaspr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2emrnmvkr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fkfbbric.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2egiqxhxl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jkylrqjy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2flpetlwn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ivqfnvpz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ugldlpfr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xijojlyi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2owjexhxj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vrlbrjhi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eqwypgzv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uymcrcat.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xxhaadwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2efwetcbf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qifaeqnq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwdmhvpe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2idvljnty.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zctivpsx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jipkkgwi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vsopoghi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vnwtjqsv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nzsufutv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mcfiniss.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2crpsocja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nogudkga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2waoskqxh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vfyfppcp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nmbmycus.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kubuhvbv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kiqvbqiq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lezyseqn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rzgkouub.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qehltahz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2niykgwvl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kuwhwwwu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ermlxekf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2exqmhcla.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wfvpkvbv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vtqeasen.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pinonaiq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yfksaujh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnhjjfl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2otftyqlp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qgkaywcg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qjkbtkqd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uagpfrrw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rbgcsqgv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lqhmcmzr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhoyeoko.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zspmouzv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vmesbted.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wkeiohjs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ngvjevej.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gnkqfjhr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2krypmqez.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hslltsdr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sytpknce.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kgjwpapw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tkgukkwf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwcnmzzi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qcknoouq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxrmstkf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xhyolemk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozdgdzhw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hxmufgrd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kjuwfmka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2obugrhxc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulovsvzz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2koperxqy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2muwgrvcn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2frbhywsf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2woivnyge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkyhier.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pmlhappc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2koqtwidv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aulmzkkb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lbyoiffi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nnrephpo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dyguctqg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ozvgwkag.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvdxwnwc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rpkhnptb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kgbjtiaa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oyufyitb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qxuxyqwa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2eizqyjxh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ivhfwvhk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uexzszuc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jheguxca.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjurbpnd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nchwcbmm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hydrjqay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2higtboha.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zrzhhpyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xemnziwa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vuyltovf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nlczdjar.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2godyxxgd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wuvcdvxh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ulqjfdwi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jkavndin.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2kfooytps.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2midvrsja.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2oqyolxwr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mkoulhyj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zboaantc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wusxxsyn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zhenhsky.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zwfjwlan.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2assbturs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2xfwghboj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cknaapat.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wgqtepnq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hvzhjqza.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpgpcjpe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gjvdlqfe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jfsywhao.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vbtgpcll.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bnrktygv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wriohspu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ssacnczd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztervizg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2luravcou.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mloesorq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fkjqhuxu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uygeshbr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ngfcvoch.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tecdouyc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pknvyonk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kpyxuaxw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdyddhhu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2uyweacep.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wkusdsgc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rblyxaop.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pnghoofr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kusiltfh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2cboxhefq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2llrtsquq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hprclrlf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxndolje.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2cxesfvcu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tvsjxyiy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nofdvtzy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wyvssouw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tgrshaie.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vlltkjry.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qnqbsuun.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qzaucmwr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gupnsuvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcyahkvt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kazcecpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhkjixvv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yoxhxnhk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2eejmaxfh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hlbrhxea.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zsznblpi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kafyjnze.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oublikcz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2odocsfwc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2sfnwmdmg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cauzvuia.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2awfjdihd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ihwzfyem.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zhpaaexg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xhqiqnxa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2aagfbafw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2luvclukb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wxoqkxsg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kchelhhp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2flnaybzg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2olujqdov.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mgitxolu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dfsdculv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wkwcmxkn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mqzwzbbn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ecxgwwrl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ivgrfxaf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2htbgnzmv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tdqowukc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2znbpjkcs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lulyvrrk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oqetoukr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fkjjuddc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cnociifn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tmsgvzcu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wfayzcmy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gxjvkznu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2btyusxvh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tjrnwzxe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yrtxzgzp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kofnbnwx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2udrrjdnw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fhknvnar.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dqfekgpd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxfapli.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gtxfbgde.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kniytdse.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nzhqitzj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pantwsih.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fggfcjgl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hbuvgjef.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fcgxtzgw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qudolemm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2chumxbkh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2turtqjui.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rplolrrk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wfjeiadh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xquixsyc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yxwcmvvh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sdncwysy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2csuwwizd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2omkmhqhl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kevwygol.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ryhdjjzv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2szaigbod.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ovxouikn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vcovvmlp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fplnlicj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rvygbsxj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ccabdsan.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qbuplrfg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fzhjgipt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fhpyzrju.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sinnvpai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdmwdkhk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nruysckq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpsmfhik.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jpothdow.html


<!-- 参考信息 -->