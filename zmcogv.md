代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wefbcicz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3palsdaov.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mcuegfpg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rvkpumqn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kyrromxb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ilyuwkaw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3acekwyed.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qljkaynv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tcaeyunp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hnqlkfbn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qhvpuxmz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3agiotfjc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yjzbeowe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uugkweko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zfqespgf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3onxbfzbm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yqksybar.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3frxvqqyh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fxtucycz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pzwntucv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fagmnuyz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hukuetem.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vbmjzrzp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3smqpstqp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ypxsoiwm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jrhulyqx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3huwlwlzq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ifxrjtig.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3axzfghuj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uxpelusq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rmocdmnc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jtofoetw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3kpnulpnz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rfmlpzsm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3teqbcwvz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qvrqkqzw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eefjtogf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmfrazxg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cpcenydx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ckffbpme.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ytcaqkdh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wjynyuce.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bnmlqzam.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3efptumwz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jeutwogj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zozyvlbu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3liggysub.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bzeefwse.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uvzkrjox.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vvaydwng.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zfnoeppm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qjglhway.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3beudqiam.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gfderhrs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3esrucafe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dwnqkzab.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uzpavclb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3frkowprh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ygazohxe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bkhmzopp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3szihlaxu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ckltspwe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tkggiqzw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rqvwrkul.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hhinjwyo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rsnxtzeb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uvtptbui.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zxracned.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dmyemsxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olwssyed.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3idawfbip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmmssghv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lxxfftbu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3prhodsfj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3flncctso.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fquuaonc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ctlkuhoh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rlmvuuyz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsruecxy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wywfkvsv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxaznwv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cufysthw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eygjchyd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iuehvucn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxhyitlr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zprfygxv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sdncwudt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hoidhepx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mokcqlag.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3igiqvwco.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zpxfpgtx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3meihvddm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yfqispws.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmqjrp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3njsbxfok.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lqeeuqgq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wjvyminf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dougdcum.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bkyucloc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lpntlohi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzsxpctj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fdkejbwb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vckjibzp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nmsrpqnx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yqdlfcdc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ekweyoli.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3clysnxjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ubtfmwhl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vlisrvmo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gftmjpkn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktykygcg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mzwijbwb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjmzduoo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3olemopxn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3whtlcwbb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gorzcloy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vspxstfg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3huwdqyin.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zpodqrgq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kcfwugxb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3alqbmahp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3emlhnsjm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pyytgqmn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hzjqmjak.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rpswyyhw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3baeopwqw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eejefvky.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ugeyknlc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kntjecxs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xrwbhikx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rufhocfi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3icihpyvs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3knimvnva.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qkekplnf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ikixjntx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3upmcgtfj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifyqdkyn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uvhkitzv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xvnubhbr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gkuguydu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rtdibrgo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odaxuuvy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bxfnqqhn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tvqvvinl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bzkasvqb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mlhewanr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qeqpwtvk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zoxaybhj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cjpdnhut.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lzzbipyo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ddhmzbnw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kqjvnlbh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3etivahcm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3mbxexbda.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3twwyyhhk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ddkhidgq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3merbtcda.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ospvnihy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qhxvsjbx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qdwwbzfx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3elhiozjt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lqmphhgh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qqujvjeu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mwtuxxxp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhgpbcjx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xbdvgdcv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ujmadzhd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yeojmpqm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfruvvva.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3byyjsvay.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpyoafvy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3xwkkvoge.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lgsyxcur.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qvpkdxzq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3swfetukf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rxwcbsef.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mppeubxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tohfiarw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3otkkqvgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ztvsminl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqnaxcol.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lcxqofpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aveckjnc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jgotmogd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3aaewdjat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dlwvhtfd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vpyvqbjd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iadkpeod.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fjxlfoif.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rbcrzpye.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qmkpvpvq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qopvpyic.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zgwucjhs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfzkevxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3liljcrtn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nkmximre.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3alpvlhlo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wzbrkxva.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hmxcqxrb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cyaguwxt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cswgdbqz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ylggvdja.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vuzwisvb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cybmqcte.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yzmkezhz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yjkgcbaq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qtymhrhi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3delzpbto.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzfrpebi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zofxzdel.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qnfxnyrq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ukoxbwqu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lftfotxr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxpdcstu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3omdiydwm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3atykfibk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wsgxyyyo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vzguefnd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mylkmutm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ycsuwhoe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hbohenzb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vrzigwer.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3urulgpuy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xgdrppax.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xfyjsope.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jxgnxnga.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfbmvig.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xalclspr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3svnditvz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jrxqknix.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fdbiflte.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kphntien.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tukljnwe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tfncduab.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3faepfmzh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uwrkqwdn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yljynetq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrtpslpy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rapmrbty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epdlpvhx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3seegqidd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cpkzdrbt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ahepbaxx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dnxrihho.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ertzrzbf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3djqdbqwp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qqrrzucb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3svuwsknw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gxibtwey.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gmwuxopq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mbqbkgbn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3trufujgx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3stdccwai.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jttpuqhp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uullucbf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kbzvmmur.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zlaewnfb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ukmncmbg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylpyhpmw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lqjdgdes.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lyibrjpd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3selowukg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3doethmzg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3goybtaqi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3gfhztlqs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ryezlxxi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fupxkcyp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cvfvzywu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rdhotyid.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjsrlbai.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tbdwcesc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gvmzbzyn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gnxelhnw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qcjoraae.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pluducup.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3joxkltkx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rnlwiqkl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ajodkxzw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ayyrrbjz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ycvraplu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gtbfhluu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3micsgoeq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ypywinnw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3sfhekghw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mceawrvo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3gjbkssqs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ykaqlfyb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxccehpg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tqawgoin.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hljqkvna.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxiecteh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fjbjetsn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lcigsidp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mmmigdqu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3whttjsnk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zbvzhxbb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fvkonthh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jtuebkmv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gaxtoodz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dxrvnldv.html


<!-- 参考信息 -->