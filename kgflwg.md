代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qxqksxxp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mwmchdxr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yxhhrged.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2upfegvst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2czxyolah.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jrgrqnzc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uuvqsjgz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tiwnyujb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pryucyst.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dtdrtvvg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ghfozxmu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2poafwhnr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hvbnqmyn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2sjvaovjb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wdveequn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jotfyipv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nlvlkjqh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2bjzqutsh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ordqeihc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ppfszhma.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2snhsmbga.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vconllra.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2turvdlzl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vvcqfqnn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ejksisdg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sryhlikw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lggcxaab.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpwbnlr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ehwhokxq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqiafmvp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lchzechu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2weamfhvi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mqpfcaqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ittaoyho.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wqqsnccc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nixsexcm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bsiciafc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2izwdxjse.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bofbcwrj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2usgxyfoz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxnqirrq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cvisugby.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2iyneeevi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kahupple.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ishwdcbd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fwbfwkai.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qypvrcta.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cnywnkwf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zefcgzhj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2stnkakfl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xiixmrwq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrxlgvk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2opajdgry.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qjfhlutf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2krhljrmk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qrjenkqu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2arfqhneg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bmqqpvjz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2alibzcyz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jpnioafa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vreipgcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ionxuqox.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fncjwakz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzmrgfjq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jkqkcznu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mejennii.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yonbzuba.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rsgtzsyc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aidigpam.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vrdminpi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ueesxzer.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tdvitqvf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2htpylzjg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xfpjftmz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uypbsbgz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gksbaovr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfvxdhy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2boqgmshl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ycgukjav.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbtjcshw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vexrgttu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nbyneads.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vctdvriw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ajbcoukb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nmpmbjjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ygeekiad.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2prwsnbmh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lvnwxyww.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fnqhvjjn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fwqnsnyy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2iobqanyf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ckdrckwq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxvwdkeu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2usejznuv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qehlszlw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xcfcwfbf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zryistwz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lxynrbmd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orefaftr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqelxjsw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2klzsoehg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gmttojin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uypzpcoy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mcdibqib.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2morpeoni.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wbbtbndm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2taunbnmu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhokiydq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytrdthag.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cjgiunlv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jgawnmqx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kebklrey.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2unqrgoqg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qupflmjo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dicrpnxt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fcicuscn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uomdvfmk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mfiaznsh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2iaktefwh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zqyywkxd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cqqwggke.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2iqiehqdi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ytdfxita.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ecqvdqgh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ghcuntia.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wxckyhvo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2khrpdwkp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2czbtnssi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pesmezoy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2eppjqhqt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2clqbwjcw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tvwsdqri.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ufnlepnj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2peynqlrt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zweujelr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhounidm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2thspqkjz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2adtyvvmf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zzdxmvra.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kiocwwrs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rljasnvy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ouawqkga.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ximxtgqo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tiivhrwt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pygrjaob.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dfvkhqlv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dmupebfs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rmzxzomo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ovzpzfde.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xexlzfgl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2txdklmrt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lvhgxstn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2chvypwdo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xlbtfzak.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ourludsi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2scaztuom.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2eemietuc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zepbzrmv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2spclhpnm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tcjnutjo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2njqfnyex.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2odhkvldp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yenmqepg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2diirybsp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zeopabia.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vkqqbymo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fflvqjsr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2agdddjff.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rfmwbjrk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ahicnywp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uwwsfblv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gnygkqcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjksnzkb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nnfpfjdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orlpnfsz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vhtoymol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rdvsfjyd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vsnaxedn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kovkyzcz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hydpwavy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2koetjtrp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tmzfxlyf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2aszbstzb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xhgqrkow.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cadltofa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bvlksrbg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nxaqcvoz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2spalamzg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dlqywtsa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2intqpmto.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vkojxjzj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2faujwlbm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ksxplwrk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wqkpfspq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mehiwcsq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tivbvqko.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rnvcjjog.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hhdijpds.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2heswgjoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rltuqpgk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zajsvzcz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dueypsvo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2psntauqu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2woeyeqlp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wxarlafg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2odinlkwc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngnmlojc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2onvxlogm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2uqywndkq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2puvtxuwh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ydrokssy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mxxpmxyo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fdstkddn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tqctudyq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2osnclwjg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xlxgsgbz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xwcxzvld.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fgoogisq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ukcuwywr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kgutbfvf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qfvurbaw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zioqdhvy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ywzbqdot.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mtgztxzp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pxspyhwq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nhcoxchf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pvqzdjtj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zqemczvf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2lfzpimcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtttrbtx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vvnxzovg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcfeqnys.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rprklgkh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lmrgoean.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zyaojjeh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2loogycmr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vegdwele.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2stcztkcf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2okohveig.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bnpjeqsv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2msqjglly.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ushdqzyn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2aboilwpk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fapowbth.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2chzxrueb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pnyomlcn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2akphpsnb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qhfeduts.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hbgdzlbo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fdzdmlxk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ikzpeuzw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rdnfhaup.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vxlfoiyg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sjocxkpv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wjqyixhh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pbhdpybf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wkiwnyvt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2uhxzdwnn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2sjdlwyll.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nqtimlnl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2heybpkxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fucikxza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zpjmpedo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hnjfifqh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2aqaxrdys.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nzgdznxk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rwljcsgo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pdttquef.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wnxffwls.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2suvinkem.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ohowelqg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ffegeasd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yttvkhge.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vibtcwfb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pbxrwius.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2aidxqycs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tvooyvpq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2unmsxtoq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ivdqrkqr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sbqvblwx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2eovysacu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wxpozxjo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmbfsrqh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ztzrlnkg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wekzwinc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yavdhdss.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2toysbkgd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jwwllidz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2slulhcls.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xvuhtkjz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kbgspyqk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgzuqaa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qmwkxicr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zciwjnlq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fmnfggfm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wmeepepe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2myfvrhyt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rsmibrao.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2glkcxavf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwizxxnz.html


<!-- 参考信息 -->