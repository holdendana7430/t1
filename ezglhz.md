代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2csymvsgo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fxewzsdu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ogyfhzry.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2agbqzvvc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yplpbbqu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2beatbvcw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gdhycxef.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zowhjikx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fzsyskai.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2iytjvxsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eqiiobtw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yrgddtbs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jotpytoi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ojmhxgbv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uavrlwde.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uwqluoim.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2brjtuaqm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2glrunpoo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rzveskzq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bndpldic.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fwoiyfwd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qgnhojft.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rueuawzp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yvmahoso.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wiojdgiv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zgzqaxzr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvctrvjr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lewqbwkz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsxetyly.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2itnqqicr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyhpcxll.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvfjsjup.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sonfxzuy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bogvkwne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kxfwptzq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmfsuhtd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xuqfeacd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tujrvban.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tgolksdt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tipvticq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lkcvnyax.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vbosoztd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vcadtmar.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fttlhqex.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2odzsqfyf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mqwqqqyb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lxhgyyhf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hexoirbp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2midafsxh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ezwuptqj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2axbqoxhv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dedtcisx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kswekgrx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vkqdrezd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qcqqkrdt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uuiiuzsc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ekxwvtxc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gqexzory.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bbuiydmw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rtstupny.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ujiulcni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueuddwsq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2soalmgie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upewupyo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2clfljauo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kijkrubh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fsycppej.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jywxxbgw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lvjmfavy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwroxkt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvestpwc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2poeiocjy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkdwvdvf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2suzajjmo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nybccojz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2axgpzvhe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2euagnyeu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fmsmtqld.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fofnkvcq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2excyxanj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nyxpccui.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qevvbkgp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eepkkrjd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2aorvqfgv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fdbvrbpg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wzdexspp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bszpwtdv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cdavabri.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2iouaotem.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xpmiohjt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uiropfyb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2eyuziuvh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aujoppuy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntrorrvd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cfyjshui.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wbubihxd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ptbmmztg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lopkuvus.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkghinua.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xhoqgyaq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lrevssxf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2knczezxs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2elwmkkuq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ghzzqnqk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2flsixytl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2awwsbkrn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwolfjbk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2diyjuauc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xevwlacw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tpmlmbja.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dolvrubq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gndpnrzm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vuzeisxt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gekxssdv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xuuycydv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ztdyqfhu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hvktyozd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2efvpqbnb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2igwjykmk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vfmeahej.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mdnsqvvp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zinrteck.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2icoiomit.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jwmpvwys.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kuoxatyt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nakacfxi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwlalt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vuoeeyqs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcfzxsei.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tukxiltn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pigwegju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nspgaacf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wmdilbcn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uelwkagt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cptkpuzs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqcqnvqs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lixohuac.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uoeseqcm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2blhyvcvs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dormqlti.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kkhfkyuf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ertgxdbh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2famitcwc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vxvnczuy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2frzufgym.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2coonrkoz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wkhomywo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hzmdvqoh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bcjzylvt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bfrcfaoe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybmbenzp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbycoep.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqgrtqz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2amrzptah.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gffbyujc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ufbccneq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gulxpmre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xosoojsp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2goxqihyn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cedtsfps.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nkgflasm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dqzyqymm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pffyxknj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jlzpemny.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ivktjyqa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2csmawxjs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2trkgvsyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vfmesodb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nsujbzqo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ocyjhjdm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qfmrhcqq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uocyqfkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffumysgx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wuzrwqwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nesxwqzq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2smghodrd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2crzzbmep.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lzfiijbx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tisylqxt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wdouvkvw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xhwxfhwe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2otkpkfep.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bqkkpbjf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xwcctase.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lbhrrbjj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ciwqnizs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jbezlzix.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dlnpkjkg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ekucoeww.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ilhawtxn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lmnlidpo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tkeztryt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2plcsjldd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bfiecfgr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywruwtsx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aaujmanh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2doutdjko.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdurrw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wozmbjyh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zcjxdnsg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pftwnlvw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuqzlkru.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wczlhjyb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qqunoxdp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2temdcyas.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2exhsiqnj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjtemdk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qrvztmoy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2meychktm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2skczwejn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gljcpzeh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2unghgoyl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qevlucqm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bbwataqe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bhfzcaul.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2glylmkxy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yzxjbzyf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hhofegun.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ezswfpfb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrxoizr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ihsvquvr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qltfgzps.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2idzgmdcc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tfwkspzj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2icpbgydh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2viihugph.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lykatahw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jxvlwdmi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2brozjfhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npevhseq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2motcpahr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fanryvvq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dxgblzzq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2popwnpkz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yxdgxnzx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zsbpgipy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mopbbdiw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2slizikbi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vrdbazeu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2arvqjuig.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dxqmtsni.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xxbkvwci.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2osolbdeo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kfytgzya.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2eegisgga.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mcvnmvop.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2esxrjqws.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vfydnvot.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nembusgi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lzczqghd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tyuoogws.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vbinkslr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mgpuquhb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2grizntcu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oetdkvjh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zrmxifao.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wwmakekq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2sfeopcua.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jikxurzz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2weywhyds.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cdioiwhj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2spqreumd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ksuiwqsp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uxquqlmg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kbmoxkei.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pyxcukre.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ajdfsdwh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yuvcixfx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gvjigdqp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ynwyuywd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ttcmtvgx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mlfjmtkq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vubamurt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nlibcqaa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2syvuhveh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gdoksqza.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nqtmngsn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vlwoplgd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hbgbrzal.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2oaaghwny.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ievhtoqf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2stuicqya.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upkgyjfb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mdjrnwmv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xcvmchtr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwzeunmo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ngahnmup.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xdjvjkkz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pcjidphf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2unuioypu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hsontsnh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbsyfojv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tyeoqffx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xrhgvcwi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2evyvncxl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2torsvals.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjvshbi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxidasqi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2olyltlcd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2peojjrpa.html


<!-- 参考信息 -->