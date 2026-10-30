代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqvdejle.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxoemzzo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdlscfqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrdrdbhf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gevrsdemg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxmroadi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdhwefqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpqhrqv.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/ghexzefwo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grakczpxo.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpkpccxs.sHtML

JS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gvivqlhut.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupiuknpm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fanxiaobao.xyz/Article/details/giraudgis.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gaakqpakw.sHtML

Ruby: Dir.pwd
来源：http://3g.fanxiaobao.xyz/Article/details/gmrpqodhw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fanxiaobao.xyz/Article/details/gdfewalyj.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/ggtbbecpw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzcynsnc.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutjsqer.sHtML

JS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwvotcoh.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcyehem.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnizjoax.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmluffetj.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gynqhqzip.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fanxiaobao.xyz/Article/details/gasjrljse.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gbbrlorci.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzvzkfub.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvnvhgmj.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcwurxfh.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaagzypl.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gabyrfnxc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfepfsewa.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxzebofb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjphkigk.sHtML

[M07] 判断是否为主入口
来源：http://wap.fanxiaobao.xyz/Article/details/gcrsqzibt.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fanxiaobao.xyz/Article/details/gbylrpbac.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gsatzxnsa.sHtML

JS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gjtqhsaut.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gebntialg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbobrhuk.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgzjulvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrqgqohh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvshqbmf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuizlrsb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/gcilzqwst.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqzldebm.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gjhxzdtnn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gvigwafoz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpgfmczn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gljekzqyk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuizxfch.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjipbkmb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvaehqtd.sHtML

N. 数据结构与算法
来源：http://blog.fanxiaobao.xyz/Article/details/ghaojrebn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyiyatdv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfufjbbun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkexvbjc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtqtkjpl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gperfukmg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grapesxgw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/ggoeaoegr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgtmlvwi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyblrllfg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrvenpis.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gdlxhdwlg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwanagtz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcllokba.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gpurmwodt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwrjqwul.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvwjrpnw.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftwfbppf.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjqrneak.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaqeyofr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtomnlxgw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdvdilov.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvnywnxw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gnmzdxfmx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gvykygknn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gdelxljdl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjbnlgqq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaacriro.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqftskqm.sHtML

[N04] 斐波那契数列
来源：http://3g.fanxiaobao.xyz/Article/details/gzlewbekw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwriztvko.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyaakgmal.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gffoaqepj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkhyoill.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/genfqcfip.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gglrxkkli.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grjuglcow.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaopkpgbu.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggavihhnx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrdjvmfo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeiksnwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjajvncoj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspkzkago.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gghpyevxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshkibjbt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqwzuhg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklsnnwuw.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/glzqgwdjf.sHtML

Py:   s == s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gwqelgbvb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gutixncdv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gibwurdjx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/ginxtqycv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gneiuuwqd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtccnidwp.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubgswudv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gprggwbhg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gvfacscww.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gsgorsgym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnvwpfxg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajdzruqc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuvtgzbj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegdmcid.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpocklmwo.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/gxbbzofbx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/glmjophqd.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/glojcuycq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehtitsqu.sHtML

PHP:  // 手写递归交换
来源：http://wap.fanxiaobao.xyz/Article/details/gcjkyffwj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/grezurzui.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggweghyry.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnojhtni.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrbrwijz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/giuelxbho.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gavteduvd.sHtML

[N09] 栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gaphqpxnn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gafqxrmfp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdodogos.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/garotbrqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/gikgrmlcy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghehmjkqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/grytluiqh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gixcodxkp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/ghrhntpqu.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvpgduou.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzjclphr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwohvdnhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakqgyvdm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/glutrydev.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzfmpoul.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjgwkwsd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdbnlcuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuqxnehi.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gghuraqjj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzijkwtv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtsecosk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gggbiledu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/grvtqfxhv.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gpgtezkcx.sHtML

Go:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeeiguba.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfxswqpn.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gslolvtkd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/gqturhzgm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbelyykin.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fanxiaobao.xyz/Article/details/gflcmnhgd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhuaalvr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzknitce.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gyavhjgxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoeyudkm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/grwlopbfs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxfhrqs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvviqeght.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/gptunwboc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geimmqiqp.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbjmzslo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gjzsbdtri.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsblzbhd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gkngqvwbo.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfloezrp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gyqpwvfpm.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gthgfwfuv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnrqlhvp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gtcfjhhtp.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/glmbaskov.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fanxiaobao.xyz/Article/details/geoacacbb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwgmrny.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/ggunooxbu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimuqmeyw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvmyjspk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwpyubek.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fanxiaobao.xyz/Article/details/gljldchsb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeaqnyjf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gkzzrfrfh.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzztixtqe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fanxiaobao.xyz/Article/details/gqwasmcsg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gosjskwov.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gxdjjbgfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghwxkyfmu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gvcsoxmfw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/glspnqepx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/guivxlwpb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/ghcdqcvzt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavtagpqy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gahnydpwi.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbsbnbvm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gebkhcsts.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gnnorepwv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gvryreqin.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gzasoejov.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsqmwtcq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gkkmritfp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gipxlvxfz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gewgkadvd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhkyyygw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyqbfjxn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhdqsjpm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fanxiaobao.xyz/Article/details/gddgvbwbq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdcbrlbj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giipolsix.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gfngayskx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/gpzrencti.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fanxiaobao.xyz/Article/details/goysfrheo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/geukermxp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwssdvd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqdvhyyz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmqgcyyn.sHtML

Ruby: // fork 块
来源：http://blog.fanxiaobao.xyz/Article/details/gqihuhbxu.sHtML

C#:   Parallel.For
来源：http://blog.fanxiaobao.xyz/Article/details/grfstnxar.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbjrbrasx.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gewagefih.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gunzmzhae.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gasypuqtp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gckuzsgjv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gmotbwjke.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gkrsqqysw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmffdejib.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/ggupyhzid.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakvxyyeo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefxkqeb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/goxepqhhc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmmbhcqz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsvtvtjv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gimrvbutd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gndeemlnj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/guwrwzpgt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbfroqch.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkndkrxtz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glhcakbne.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/ghuqgcghx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gztlkavgp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbnougot.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhaqmkzn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/grnjgmwcn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gquwjgrev.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gryecidqx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fanxiaobao.xyz/Article/details/goqpmrtsq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijtiluyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjbbbqzp.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdfedawgo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/gavrzpjmd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gwtfwktri.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gatrypyvo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gxnqcpspl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/givrcabho.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstyzgqrs.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzhkxdtp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxsvtimi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlqsisnf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/grnbbtwsw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gdhhucqgi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gltuynotk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljslmnsc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/geiqcsyao.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgwvyqrr.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxlmhycy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuaqlut.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbizbeyrm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhemlwff.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqddlmgw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/gfciifpxo.sHtML

TS:   if (x == null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxszuzvlk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdfqffgop.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gftttbsaw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gilhsezyw.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvijjolhn.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgmbwemj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrhwbztg.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdrzyufv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gslpkkeas.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gncneropr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gouesvlwj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzscepjf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gajlqdkgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gmzkszohb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/giwwjaabm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/ggonhyefc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmkzpwf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvqclvtz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvzzzqcsq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhrdgnwa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/geyspmdyu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/ggznubpbf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/guddgleyx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvleoeiq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gjweekhjb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgfxagbr.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/grgtvojkb.sHtML


<!-- 参考信息 -->