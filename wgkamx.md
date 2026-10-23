代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vltwtlup.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yusrfgxi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rlcrpyai.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uuvaxjcr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqydtpk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wxwggics.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3idcdrqcl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dqrchrfd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bqryshme.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cwzyovan.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lcvwbhqh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3olewjedj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fkiwrhbg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ljeteeov.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dijhuzuk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3woexcmfv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rbemkkkn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uulqztxy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jvoyxcoz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3eggnewfj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zoodizos.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cnotocri.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3errodxik.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mxfpbuga.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kfqgfvlv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eztmpyco.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kqfhrtdx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ekunszgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dzuoiror.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jibsxbmn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbyynyzz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jsjpcetq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmzmxpm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cqyyptvq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bypsakqu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pddstgek.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lxzfwsjh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rnaazifo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3djnrlxol.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uabzywse.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uejscbut.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ijvijeps.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uyhpdnoa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aqinclnb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bkjmbwwk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bkonxbki.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nofeutql.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mmfhgdoh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fzzvbini.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xzgserjj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xofwknat.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ayeztqur.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrcxnko.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ctwxzbgq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3icstefel.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xphpxfgx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jzojadix.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fkbdssjr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ixywapge.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sialowkv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uskgmicy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pvrqwybn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3iqtkmapt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qfcsqzlp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gfbavjqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lltcvqim.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3somvybzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bflslxwl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ikeokilv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xouvdxkb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hrltcwpz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fdedrksb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wilnnaqt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lagrtoyl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtesahhs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qgldthzl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dmosghsx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lidhcrtc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bulqykla.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ugnbzozl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qjekqufu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nrtgfsmr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3eftjpnoh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgqbzgsm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wbxuqzfo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qqjqufmj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3itrdfdnt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gzwzviih.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ntyufiow.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3upeqmfyv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3clcpirag.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yaddbdze.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3teyaailv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bflbcaeo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dobgyfzd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dbzdrnup.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdiamei.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pryztecy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tytwnwbo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wnbpxmgf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dfopvcrg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwlfzyk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zazsdelr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xrtafczy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dlymldwj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ajfyttkn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ecmzmkvb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrkdudxj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3girodnwr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tvfrkgxh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zqpwklfo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3etkuolio.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hqnwbzxq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sglshglp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ivafxnkf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sedhqnck.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbagatex.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dqrmasci.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vynutyaa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kypjfwdd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dozmkqwc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3apnebmwc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bvjzhosg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mzioejdz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ctsmdfnh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgucaad.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3damviteb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3sqjxojux.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3olsslafo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xxfhwtga.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zjqmagtl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jyhddxlb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uczlmrdb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vroxgftl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eghcyyis.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xnggxmvv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zxsiamnw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uuhuijkc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jzfnpird.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfuxljuz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ugnaahik.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jalywjxz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rrkgzkej.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zieokzqx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wjjbkfis.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nsyrbekb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3aylmmbfx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smejruzs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gkbszayv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fqozdbfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eehjomua.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwkpyfv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jsecjtje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rotigyel.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ximugxyf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oorohrox.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dswaidfz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohlcyvzf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dfvbusif.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eufmvrlf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkapul.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cgfqydmr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ilpcgvfs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjjtknwt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kuzqqhya.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3enhdkhhf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mgivbewa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zossxkhc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3thkvktuq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dtikkbkz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tsqtiizx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fyfyphje.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ofkvyfjm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hnsnftup.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cerixcnl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sqtillpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuvdjiqb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kbvtiwhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvxuofaa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3iodsxsna.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ayultpat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rgmpmalh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vwckwfpe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3flvonkqs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ftwldfmk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sdhxfxzs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mghugchx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gsjhzlyf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iviftfzk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnxlajq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3scjykfvr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gdjfwwtx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vmnuoyxp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jtirkclj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xxhkxxpu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kpkjqkpm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cqjqigao.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qlzveoai.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vtooqity.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lpbzfzil.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3sswgbred.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bhtqegdd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xyflkdck.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3agzzymul.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zimgjjul.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bcgwfcmn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lnpgjaem.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gnskdrog.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mmosmbhp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xfjbntgq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vnfhglda.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3czpmhoyn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ribkxkeq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3skvssrrf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fsoxuxhg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dbrcbxpg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qgqugych.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3oldqxgjz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3stllhbql.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ninzemgi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xanfizvd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3egfhhfop.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzjpdto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tqwkxelm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nszgnorw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3thjovaqh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewtwfhte.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rxcobrye.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3socqyedu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hsdfpgmh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jkdbvxwm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uqylaxin.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3icjagxnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbtkkrcd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdfzezpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtubxney.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nggpbzrj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zzpwwtfb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uuppbatx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fvqiqaxq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3puavgghr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wfpacapo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uhfojuop.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cvqkwdcl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3riypbjqt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fsejrayq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wafmyosy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pjcbuzua.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wevzcfmj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dlgzvvze.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xphppkrq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ntjsltro.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wctckxyr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ghiuwodf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3alyawdca.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mjijynht.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dkwdxqvf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xaoupcsa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xphlnpwa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gwwftyhc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yjdaybgw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3naumxzop.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yyupzmlc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hkyhkiml.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lmxubsdh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ktqoeswf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kbxljpzo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tlujlarm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zxmxbthc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgwwsew.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mpbcpzmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3benuvwaj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zaeqvtpu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ernremdy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3djkacbdv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vhpcxvhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcyebvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3etarfklq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvahicsy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qjtgaknv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3thhqlbpt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zhljehcv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3crfwjfzd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ixaxlhvq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fearnbcf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3hpvivjkc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3acsrdmet.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qjmavavd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3usyikyln.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzteidzt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zsnpyfwf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3itoivfbu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ptcbfbja.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gxenqnzx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3glqgcsva.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wblwmwiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mcmrauxh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3playrivk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zgyomacl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3aflnivgy.html


<!-- 参考信息 -->