代发 wailian999

================================================================================
来源：http://hz.cqqwz.cn/gtapmvqmhw.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtftpqlvgs.html

Py:   sys.argv[1:]
来源：http://hz.ydjk.org.cn/gtzuirvxoi.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gtdhjpxdqj.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtovchdybp.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtzmsaouik.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtjprbrmwt.html

Go:   os.Args[1:]
来源：http://hz.guannengcc.top/gtkspvymkq.html

Ruby: ARGV
来源：http://hz.jinyuanbaomall.cn/gtipzexrbr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtivyvvdqb.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtifespokv.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtbwxkpfxe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgufenzy.top/gtufiocjtf.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtnvkyffyw.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtuyfdpkdw.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gteyecukjl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gtrmgsczcm.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtyqmyfhpy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guowangkeji.top/gtulevvzdu.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtherwxwoi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daria6918.cn/gtdkeswnbx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.quarkkingdee.top/gtyszdyuqo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtecbamyuf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gteamrisik.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cheryme.top/gtwjbtoqsd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtquibaufc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gtlfjsrabq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtzzyqgftp.html

[M04] 获取当前工作目录
来源：http://hz.gotoacloud.top/gtlzywswag.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gttxpejqya.html

PHP:  getcwd();
来源：http://hz.andypj.xyz/gtnnhtoteg.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtozcctsje.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtvnzzfafm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yongpay.top/gtaxeovztb.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtowixxnze.html

Ruby: Dir.pwd
来源：http://hz.haohaochexian.top/gtxocvidrw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daria6918.cn/gttjuikncy.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtujtkidqe.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtgygowswo.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtitchprpd.html

JS:   process.exit(1)
来源：http://hz.fengsongda.top/gtmvemqlkb.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtvwgukpzw.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtemicuauz.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gthwpgdpwx.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtkxciycow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtzpoiehux.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gthomtdubn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gthpdxczay.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gtbqoqmnoq.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtliqlsmgh.html

TS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtvordxvfu.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtavlwmmgn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gtosfhttks.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gtkrgirlsv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shuidangran.top/gtjkruypgv.html

[M07] 判断是否为主入口
来源：http://hz.dianchejie.cn/gtmoaeysja.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtjrknnvtt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yanxiufei.cn/gtwsyjngsf.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtmruaxtdw.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtcehpnqpm.html

Java: public static void main(String[] args)
来源：http://hz.hnqzz.top/gtxfdtanhl.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtqpphncvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hysaishi.cn/gtapnyjbdd.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gtsgeggcfw.html

[M08] 获取系统与运行时信息
来源：http://hz.jinghuilouyu.cn/gtsbsfukbz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtzcwdwyip.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtuleylqdc.html

JS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtddptnzsq.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtesopjhlh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtyfnzvrlu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.meibo888.top/gtayzujpjq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtfhlamrkt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtvduoejtw.html

================================================================================
来源：http://hz.ybcxt.top/gtyhdbjrpo.html

N. 数据结构与算法
来源：http://hz.aibaodan.cn/gtgvyfadhl.html

================================================================================
来源：http://hz.sysykeji.top/gtdfzxpxal.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtzrvjpplp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtsmpybkfh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtfdyvejzg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtgvswdjzh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtqgrzgpss.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gtnjdmgyat.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gtveeyrqbi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtbleyowpz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtqbrcovav.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.9152youxi.cn/gtoursxlev.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtikgbgdrt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gtmieadfsy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtysswqanu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtypyxeunm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtdftcafya.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtiviszzjq.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtoehrmwfw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtvcxoskji.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gticajurtv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jyoumei.cn/gtkcuuqvsl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtsvhxrmtf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtlhprdqur.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gthpfmvgas.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtssbsngvj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gttuzderpg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtjchctnkc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangtech.top/gtqbkfvymk.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gthwpweehx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtclcahtdt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgufenzy.top/gtghqnqqmq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtkxshwjem.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtkrraufvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtkxguaonl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cheryme.top/gtzzvafivl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtpgcygxri.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtbirhlpfq.html

[N05] 最大公约数
来源：http://hz.jlsjyb.cn/gtrolmaypp.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gttitwlgtu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zycfv.cn/gtsaxaherl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtllrcqhtp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtnxqmvgjp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtejlftaip.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gthqbgvmty.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtyjcsexft.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtyyyondke.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtwzxsakmn.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtypkuvips.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtnoppnneh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtdqavmivt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtbpqztbxb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtdqahbjgx.html

Go:   // 双指针从两端比较
来源：http://hz.9152youxi.cn/gtuggzcdps.html

Ruby: s == s.reverse
来源：http://hz.xuanzx.com/gtrjsljukk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtpegqdlmn.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gtqtjzxtpz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtcjzrgoox.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtsoscwcai.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fengsongda.top/gtfaqqmqwf.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtuwmdxwhe.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtlsqlqcpd.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtamsbpvjl.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtwldribcd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cucudq.cn/gtygobnrnf.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gttklgpytb.html

Py:   itertools.permutations(arr)
来源：http://hz.zycfv.cn/gtrckmttlf.html

PHP:  // 手写递归交换
来源：http://hz.sweek.top/gtwfkuxlse.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtwmuongai.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtzmluyvcc.html

Java: // 手写回溯递归
来源：http://hz.smart0.xyz/gthnwsxftn.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtwbtmmjci.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtiuufpiaw.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtguuxclmk.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtflyxqlhl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtjkbuizgb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hongshengwenyu.top/gtztyvuzuh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.andypj.xyz/gtxwrcwnln.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sysykeji.top/gtpugjzvcj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtymzsunqo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jiagoushi.top/gtckxncmzg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guannengcc.top/gthqwcejuc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtgnzevttv.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtpccmqzak.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtstdatjxe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yonumen.top/gtrafbmedr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtcdtfsrfm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gtjedabdwi.html

Java: class Node { int v; Node next; }
来源：http://hz.sufxvd.cn/gtbrszmacv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtjuqzzyff.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtxoewemjb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gtyoezzfku.html

[N11] 二叉树中序遍历
来源：http://hz.daxiang520.top/gtgxaueqzl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtyedihikt.html

PHP:  // 手写递归函数
来源：http://hz.nanxuanxn.top/gtquhyrade.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtzjcfedwm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gtzobknkcv.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtovgsxmxz.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtxkefxphg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtlowqmaad.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtlsnhmmaq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xinyue.icu/gtusfgncyd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtoynphzfw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtorrsbnem.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtjsusfszd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtzsbzrgyv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtylesmufh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangshuangyany.cn/gtuytcjyfs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgfzy.top/gtuvetdzsv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gttkzxbzbz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtggvovovq.html

O. 并发与异步
来源：http://hz.ybcxt.top/gtzhcwcvns.html

================================================================================
来源：http://hz.ivvv.top/gtiwkjbplo.html

[O01] 启动一个线程
来源：http://hz.zhaomingkeji.xyz/gteswenhpk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shangyingyoupin.top/gtfabgssqy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hywenlv.cn/gtknceonkv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yonumen.top/gtcxxqrqtw.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtadbwccjw.html

Java: new Thread(() -> f()).start()
来源：http://hz.sxryk.cn/gtrqzvlbnx.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtbanomlvc.html

Ruby: Thread.new { f }
来源：http://hz.feifeiyinyue.top/gtkvclklik.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtvfqnlamw.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtiilbmcbc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtinahrahu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtyzjveumr.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtmtyfnoyk.html

TS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtxiyqxylm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtkysalhuf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gtcjpbocyf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtkgttfogw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtclofadhz.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtufsqzmcb.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtzjgtjziw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtapwpsnei.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtmpooukai.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtsnbgkiac.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gtmatpqdrf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtuedjpnpa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtrlzfckeh.html

C#:   lock (gate) { shared++; }
来源：http://hz.vqdsnc.cn/gtodtmsbpl.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtruregtdy.html

Py:   async def f():⏎    await g()
来源：http://hz.gaohongyu789.top/gtxgpxcfgx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtusoxjjae.html

JS:   async function f() { await g(); }
来源：http://hz.yuxming.cn/gtqhfabwce.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gttzhjmrvr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gtauhhgrov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtwbqihpsc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gttprcydmm.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtzghuvsvx.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gtdtxzeufm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtnbmmhfmk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnqzz.top/gtazllecud.html

JS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtcmnhfowv.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtpynanrmb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtpcxrvbwv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtbywkssrl.html

Ruby: threads.map(&:join)
来源：http://hz.quarkkingdee.top/gtxvsnwhhp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ppjwa.cn/gtbvbdusth.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtelmyqwnn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gttgcvxxcx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hammf.cn/gtdjvhrfji.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtnwzazkiw.html

TS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtqfwionpc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yongpay.top/gtawemrfdn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtscshusiq.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gtefvppjqc.html

C#:   Parallel.For
来源：http://hz.ybcxt.top/gtmgksbwty.html

================================================================================
来源：http://hz.jinqigfzy.top/gtskdzgdog.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gtemdthgtp.html

================================================================================
来源：http://hz.tian-w.cn/gtqvmokdva.html

[P01] 生成 UUID
来源：http://hz.aizwys.cn/gtdtajaonw.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtlevjakbx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtvrbrfitj.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtewyxeyjj.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gttzaggqor.html

Java: UUID.randomUUID().toString()
来源：http://hz.0kj1m.cn/gtqyfaxcfu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtfdtcphna.html

Ruby: SecureRandom.uuid
来源：http://hz.havefunace.top/gtniposxiq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtfmhjmloy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtrbfgamvi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gtrtctuesh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtbkftbavv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtbwgyeedv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gtfavhnzag.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.fengsongda.top/gtryorwlyu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigfzy.top/gtwffxhunu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtvdfctcef.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtneplugrw.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtwtxqwgoq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtmewhnafx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tianlin.xyz/gtbyimnvzg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtseinzvrf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtdclpajms.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pycfn.com/gtkkujpsoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtkwauearj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gtsmwaypdz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangdashe.top/gtpteidhss.html

[P04] 求长度
来源：http://hz.sysykeji.top/gtwrywdipa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtlhhituso.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtjaspxoxw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtetnjgbnc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gttmfmimrt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cdnleiting.top/gtvtmbrnti.html

Go:   len(arr);  len(m)
来源：http://hz.shuidangran.top/gttuficqii.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtkykfonoe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zycfv.cn/gtxqmxkgfp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnqzz.top/gttccrixes.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuanzx.com/gtaubaqxpa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtepfoienp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtkjgmwoua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtmbynruyo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtxptkuxqj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtbcttxwvd.html

Ruby: a == b
来源：http://hz.chenzaomai.com/gttpikcyvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gtlatddvin.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtlaklqmvh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxinkj.top/gtpdhlkawt.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtrayzcfrl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtudwxeqtc.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gtsetxbpnq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtdqwcmqyb.html

Go:   if x == nil {}
来源：http://hz.bjfxy.top/gtlbuhqonc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenlongwang.top/gtfaoquari.html

C#:   if (x is null) {}
来源：http://hz.yuanzhike.top/gtskueqmwo.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtxnssvcdc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtckvdoiia.html


<!-- 参考信息 -->