代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2epvwytxf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dhjjhxiq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ndzriqvo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vfsjkasz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xgzajmnu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hngcuzdn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2grqhttvw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xxknddno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eqxwcbfg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zmmtfyju.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nvovtann.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kftfhwfu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xopldsrj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wnfjptvf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kpogbmgl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ullwybqn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tzblqkxp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aszeadcm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sjumjzjv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2noxlbgcf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2blosufjb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wveapwxr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2omzqebwe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dxkaiwei.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymczwfhi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dbdabdfj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pudbzxsc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ickxqezg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ziigqhof.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xqnuorlw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rbfcumwz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gavlphxc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2liuqtuub.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdwnkus.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hhdsgszj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eimuqkuj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mcavjvhd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zvjnlmuz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mxwrlnvs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ueherabx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kcwmqrvk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ovxgujkw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xlescklb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hbqgpuuq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2aognghtt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2otaskzbh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lmnkiskc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dijpgaqx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iftauqsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2nvqjrlwu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ejwvbhyj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wsfeaqdu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhfcujb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2yzlcmrfq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ocsvktnu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2csbvnhjf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zgnpmkvl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2evvzvxmh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ezrfnicm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vvpfzmse.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hmwdvxyh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2roouezxh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ttoirzdm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mjliqgii.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ojqzqsql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfhnoqxt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kviqgnih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vosqlzxd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2iaayrvmn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2upnnwfdv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dqflxhjb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2spsbdxha.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hzutwubg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qnoxmwtm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qudnrbop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wwuqxryc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bnoeioux.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kctkhmyn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ozafljbt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2iakeivqo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zopjgffp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvuwtweg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2njxyzlpz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qshxwdah.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pmrazqxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mtyesaui.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jqzoalhx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yrhjnfjs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fxgxskuc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sggfmxno.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rdkqxnbc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qktptnns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gptqinhe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2prlamqxm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gzfvguei.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2idgmxtsi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jjuunggu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdqqofuw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2shfrdlsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wxpzgyey.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yclvxykw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2clufwucn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2atuophgx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uitnfhvg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qhstjonz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2focefhlr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jihhhlsw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bslcndtk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tzmaihdv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2floyhrcl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kftusank.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ddawofiw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2skfyxezu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pduzbnow.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mcydwbzz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uusuhtwy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dksmwrdo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zauropra.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fzgnzejt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2koqbvflp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nfxvmjgr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iwaeduhn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wdibayyf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vejpqwyd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2totikctv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qzgsekgf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ggxeanlo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ytngtgjw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dyzbeakt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2khfwvxuz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2efeuwgix.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zjwranic.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xswdgdhx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qiehtglv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zszwmoal.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uvcpukjm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xpjjyuvs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dpqjiuoj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2juinipxw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2exmzzuke.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xfyfyidt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zggsjkng.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2usfgiawv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cwnyxxwb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cdjlulkt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rmdsssbm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mppdphac.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yflgqdcr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bghofmuw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hieqwwhh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2brzxsdoe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2javrzjzu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jcmaamaq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hnvpbmfe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rabbfyio.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zcddecap.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hfbbpsne.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mililwbk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2uvflwalo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vodlassg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yjnvxnoh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2picnxojj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2geoptmux.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ccpdxhif.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hrpoctxt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ndcktsiq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2daajdwcz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wghhsrcx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2puqblnnq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zbkiplja.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ihlldixt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cqqecybe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rfawqxti.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gffnfcip.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2afdylima.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2noumacmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oejtxvlj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qwjqappa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdhhelpf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bdcuvwbj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mvpulsul.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lpcpydqk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xrowkvpv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ofjjmjxi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kquaiyss.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2phmqdsxv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kkylemrb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wqurihdp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2khfsioqk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fthkbolc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2thqjdmsx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gwzirvvw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2duhmvjpq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uufomtzq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vxzdzagc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2feshbjzf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2knnepatd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jgscbmbb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gpednady.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xfnifdse.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dupraexe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jpakbcuu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilpepdcn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ggatsydw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aqbazsam.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rhqmgsbr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2icdhluyc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vgjzuanh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sofxiwwy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fpxjedxa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqhahevx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rqschrtt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dyksnjpz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pbduiwlq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tojppvrb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qyzzugta.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfftzdl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oubbmuff.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rzfulioy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eehkorqz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2srqobfov.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jubqrvot.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mzeurwzj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zusdhiye.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2udfthfge.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2azjjrseg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2apdgntxw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2udtzcpoe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uhfurbrf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2weeqcpek.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ojeiibwm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qczxvfwy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fftbogbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhvvioaq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezithjfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzxkuhuk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qiorhcov.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lgzfcztj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ibhhyygk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xgzhisup.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hiqyjfgl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xgzfbqfh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2iopvusyt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2svdzljzv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lnkkpqiv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2khiakhhu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ovzvwfrw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ppplmrqg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zfbacywb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhoehyt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nqoldyqp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mgfqwebm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elhcjbxu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2enoavydg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mubykfxt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nnnzyqgv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2newyygbf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qlnzroau.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zkmsguvm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mgyytrvy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xixshqcy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hthnmpvp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zqhtbtls.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lnmliwqo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rkcoanws.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ootzdavm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ztmogcrt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ibemhvsj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nykdepso.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nbywhcek.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hvxzmxay.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dbellwcj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nhnsjeci.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kzibkhiz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pmsnjprx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xlvlvtgp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xuoiuxpm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yriknbyr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2haphlwif.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fwlyksuk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vrexyvyq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2suonnetg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gixftqva.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzfasj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mrttkpes.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ofjeqnzo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbtjufkv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lclcidsd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nbgkgouv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fccrcwrz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wmvvpdyj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2erraoibe.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xonyfwby.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pnqlprvn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ayjoteob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vayonjum.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jbxeshlu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ikjlapol.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xyizmqqk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xagbezxz.html


<!-- 参考信息 -->