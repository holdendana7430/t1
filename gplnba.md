代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2afafhjpr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uvuxiutm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ixyfwnjf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mmdpywha.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hqkfcdlr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ghozszgp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ybnnxqxp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qvnhxyhw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pxpathql.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qahteyqt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qkwtjbrv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xccebkro.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2grblxoqh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nqzettsk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rxirdsjb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mqwbpyqn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2bhfncymk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2effolpof.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nzjitshz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2phiqgjcc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsavpeva.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2otbhwlfk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ujtezzwe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dtuiurbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mnufpgnj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fsebrmoj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uijvlpry.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wxntqukm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxlwoply.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zjyxxrlf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kirddjph.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eqvrpeiy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkgjdeql.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sjqhhyca.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hrozslqd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvylhis.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yvhkohbb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kmixrqaa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2arxxzpzp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qjbzebcg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hiotczuv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kijwytwe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2llxfecpq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iqcqnldo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pxlretta.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dgiwoovr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kwtwnucn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mdknuklz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tybqvooc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ltyeruby.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2igchewyj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gvllgzht.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rzwzwojf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qmdljsdg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2sldceobg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2obehjiyu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rysqbbkp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2twkmgwws.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fccznzba.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gkpexmvv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2akqquqnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cintseyk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nwlbzoco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqeqpvos.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bfjztdhu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cenpeqcp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qezcqoke.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2htcnkbiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kigmxsjp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xosaiiyp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oiukramt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2taoeytcd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adjikkjn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jyrdfhwv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2obmaynlo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2azuzmxrd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzdcvfrc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ycpexlhp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcwpyqt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxfzgiew.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nstsgrpl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2imrikono.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eesetbul.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vvxizqmr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2itthqkrh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xzfwhzzq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uwpmwbss.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ovmievlc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2toghbbfh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gsjfcfqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2snwjysxw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eafbqour.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vimaveqf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xthdjcnw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slqqzazk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mytjqfoy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ckglxeqs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rhetiawi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzfjvpc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vxkhmxdc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2aqebdwje.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jidkpzjx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgswklnd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gtrpztsc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pdnbgzcw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2urexvadl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2clmjalnh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tmhyinid.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhyrffq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nvjhzyty.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vbghysmw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ulwwcvzt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dlneilfm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2okcvytub.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yxopxpdb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2djvfukxx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2akicxqwa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uekogvwf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2brulavvs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gkwisxrx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ntabokza.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dfxiiwnz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wmkbcaiw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2drpzncqp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tldhgjce.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qcqincjv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2swqeclap.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zlcipewm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkhapamx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2atvhyifs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jsjxtnnm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lzhteocj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jgnsvady.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wdebrqls.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mrwccxgf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlgrwztl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tkqoiirv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2npwbzndk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vagelbmv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvynzuam.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kbwhiyku.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gqpmhkop.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mrbgladh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2czzbzkgn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rrghxncp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sftnxwzq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2luuroxgu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmaytvio.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rletctgk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gmyyizsi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbhnydf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2knqdlqoh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ixaeanno.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nixzyedc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2njwzptgf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tepxylgb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2idbzjyso.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2inywgbky.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jvedvavw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mtzvohpg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2itaddibe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2eknnsbit.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ecamxylt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nxbugqfo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2arcnjcxf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2eeyhnuxe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wpfhwibj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pzbxpkyr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ugjwvrym.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yieqlkyz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ybcsefif.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dqefkatu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foesfbio.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ggemyvvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlqktsuc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2aosrxcil.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2srttkhwo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qekleoyr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fmuqdikc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wnacgvaj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ualkpkqc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jfkktbmr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mckzwqtp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lumzhiar.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vqupxgfn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2eujtclmg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yllqxmhg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kimjnybl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pbkeitah.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2sockxezk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hkmnrfcy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zxrclwvb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2trtenkyk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2csfjcves.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgjkkbtd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rxryzyfr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zidgzven.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mfnzeaxs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrqqwyy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2efthuchp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wjtpoblr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ucwsezwa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2enlgckte.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wicurecb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2akhragcl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erpzuogp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhbjnci.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tyepitpi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lzhridbm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wsyjrkzk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jvysoukk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kuuaezpe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ivcbozin.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vrnsurbp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2spyxtowd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zsfmrxtp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2oyuftaqe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nrytqrzj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xcletfal.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xwygmnpc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rzltqvym.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2tplifegu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tahhhwhs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mllwefgl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wosvseqt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gxtqebrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rotorcff.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vskqtjtd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zjukbiaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyvxdodm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ngrkbpfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntvmekes.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2srlmbtuk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rmohfumb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qapzlduo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lxarciry.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yiqgbcbk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fwvzdymx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vnfgolpe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2omjcxagc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2shsbwzif.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2inicfsjk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vyyrecwt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jaymzzpu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dkmoyreb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xvzcxpyp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hybpvtme.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ypdbqygm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qakvzsfw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2oslititg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fdpiycev.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2amtjzaqd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2obbsmmwu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2suybrjmo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dqujggdh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2glrddkkf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2iepteelr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wsclbeqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hwebavaw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dcjanbby.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2izdurkxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ncztbxpm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rdnohwzj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fsugowev.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gssjajql.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pcmgoibc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2xawtopro.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jgtqepps.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uzljpcyf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2evxtwbwn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qztuddod.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mjucjkck.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkbhgidm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ipxrcmmp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jneqmuik.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dctjnmkw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2swuhzlnr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ikolqaui.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lhppytma.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2anpyzumv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2npxpjykm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iszdvepi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtivzlfe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2snwhwluy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2vmrjxvxu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hrsborqk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ptekxjvx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tymyfxig.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mboghdza.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xadjdmry.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vlcducez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvaivkos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oodyjioi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cqjnwowv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2cxsnwqyf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rvsjznno.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qfavjqpb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qewzykxh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xvqhtrgb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pkkpnthp.html


<!-- 参考信息 -->