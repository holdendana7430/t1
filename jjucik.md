代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtammjpwzn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtylfepmnw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtovlwmlgo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daxiang520.top/gtjkizdoqy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gthlgrbqhg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gtjnnzcrye.html

================================================================================
来源：http://hz.redwolf501.top/gtdfopbltr.html

M. 命令行 / 进程 / 环境
来源：http://hz.feifeiyinyue.top/gtljtqyftt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaqlryznj.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtjbqvdusb.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtbswmwvsq.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtbijohryi.html

JS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtrobmurgt.html

TS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtnxkbugyw.html

Java: args 数组（main 方法参数）
来源：http://hz.zhijiandao.cn/gtzllvqxdc.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtvavdlxva.html

Ruby: ARGV
来源：http://hz.hammf.cn/gtcvegixyk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtekudfuxz.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtqwrdhkyl.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtdvdvoulv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuanzx.com/gtecihepsg.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtbnruksdy.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtstyigizr.html

Java: System.getenv("HOME")
来源：http://hz.ybcxt.top/gtgovgxjop.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtykpigbvf.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtntqtushz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtdbkvwlmo.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtbpvbbjox.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtttwvtiyk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtvnejnonp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gthrepkupp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtkqsepiri.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtlrqmwiql.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtxsfgspww.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtxfrakjhw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gtufhagnlk.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtkcnhicfo.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gtvziaxtry.html

PHP:  getcwd();
来源：http://hz.hongshengwenyu.top/gtbhveljjq.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtvrqnvhvi.html

TS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtjzvpwnth.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtawgctmwl.html

Go:   os.Getwd()
来源：http://hz.0kj1m.cn/gtvmittoih.html

Ruby: Dir.pwd
来源：http://hz.yueranfly.top/gtrzzspcsu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gtuexytlzo.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtzwuyjimz.html

Py:   sys.exit(1)
来源：http://hz.daxiang520.top/gtosnopvar.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtfhvyvlue.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtkvtickfv.html

TS:   process.exit(1)
来源：http://hz.meibo888.top/gttopnzrmg.html

Java: System.exit(1)
来源：http://hz.zhiwuduotai.top/gtsentabgw.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtezhjvsab.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtyhttdqbx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinghuilouyu.cn/gtvdhfbkxa.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtxaqxbwvt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtftmhiuny.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtqhdefmkx.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtuckinsuk.html

TS:   console.error("err")
来源：http://hz.xziqi.cn/gtbdgreafb.html

Java: System.err.println("err")
来源：http://hz.gotoacloud.top/gtcoxmjuvf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtlpasagey.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtucltlsjk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtrxveqaje.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gtqtumllod.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtvwuzqzco.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnxiangtu.top/gtscadvqxm.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtmryloldj.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtzrvkzrxo.html

Java: public static void main(String[] args)
来源：http://hz.xuetiantiany.cn/gtygwwohrp.html

Go:   func main()
来源：http://hz.zhoulong.xyz/gtlwzgcacu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtaqqtlpan.html

C#:   static void Main(string[] args)
来源：http://hz.cashguo.top/gtjgskuzjz.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtjywcwunw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtlypequxi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gtpeqtoacu.html

JS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtddgsxmiu.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtnqjsiyar.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtvqbajnon.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shangyingyoupin.top/gtibjcpqoo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtygryshtt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtpagzequw.html

================================================================================
来源：http://hz.dashuyun.cn/gtbedkyjou.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtooutpvdl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtdfhqqweb.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gtqivrxlav.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shangyingyoupin.top/gtqarnuyus.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tian-w.cn/gtcoskwiry.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtfpjhsfvd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtnqjkxlgx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gtkowxikub.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtbtenthic.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinyuanbaomall.cn/gttltjtbpo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtkhoxocdy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hammf.cn/gtvvcqlfay.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gthbimaufs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtkrramkos.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtxyzemnjy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtboyvburk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtohremckt.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtbxhaluqi.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtiohgddxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtcihwvlug.html

[N03] 快速排序（分治示例）
来源：http://hz.cdnleiting.top/gtapzbqede.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtbvcmkcvh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhaomingkeji.xyz/gtxxiofekg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtkyfgyrat.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtbfammshp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtfpahqnyq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtqhubxraf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ppjwa.cn/gtcbbeiiyw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtfvtfsiyh.html

[N04] 斐波那契数列
来源：http://hz.xylfe.cn/gtkcqdjdvg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtffrkyiol.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gttbkacbxz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtfjblcgaf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtulqleiui.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtsidjxuoh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtbwgxyyur.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtvmtnsnvl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gteufqnvol.html

[N05] 最大公约数
来源：http://hz.mhx1999.top/gtabyzjcsh.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangtech.top/gtrwqvmeyp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtgshafpoc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtlyupupgv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtxssirphu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtobxhgwiy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yanxiufei.cn/gtlhziogjg.html

Ruby: a.gcd(b)
来源：http://hz.daria6918.cn/gtxtjxtnih.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cucudq.cn/gtshwyliqb.html

[N06] 判断回文字符串
来源：http://hz.shuidangran.top/gtzwkjlqfa.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gtedzphxnk.html

PHP:  $s === strrev($s);
来源：http://hz.meibo888.top/gtmbufvuna.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtjyjckqiz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtkntschxu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtpaskwqbb.html

Go:   // 双指针从两端比较
来源：http://hz.nanxuanxn.top/gtjcuswngt.html

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gtphhyhmnx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtllqxwyym.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtewsorhcp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtrvosflfv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtgdrvvcjk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtbvyouaqz.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtaipnalwh.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gteeoyvwkc.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtffskylgx.html

Ruby: // 手写 Hash
来源：http://hz.andypj.xyz/gtzzmnuvsr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gtervaeoby.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtlluxbyht.html

Py:   itertools.permutations(arr)
来源：http://hz.yvedp.cn/gtjoaijzxj.html

PHP:  // 手写递归交换
来源：http://hz.quarkkingdee.top/gtmvrkrgba.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtubpihooa.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtwjnbwveq.html

Java: // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtvpyeeqfr.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gttjanuczq.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtnbbusqbm.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtvwckgrbw.html

[N09] 栈与队列
来源：http://hz.daxiang520.top/gtczeahxzc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.meibo888.top/gtnguzswcj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtmokzespc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.0kj1m.cn/gtubjmhlsd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhoulong.xyz/gtcelmhude.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sweek.top/gtglrmhsxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtllvlhskn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtsdhuluyf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shuidangran.top/gtzpqkahlp.html

[N10] 链表节点定义
来源：http://hz.yangfankeji.com/gtgwysgmin.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gtazdnvsap.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtlmlhuoaw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gtzveawnad.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258888.top/gteooszgns.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gthcmaqusy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gtohxdwtdm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gtewgxoxso.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gogol.net.cn/gtrnziyckq.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gthrzmbvnm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtsoljptyi.html

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gtvqftigbi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtrrkmhhhj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtkvkjsmsi.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gteukjomtm.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtbwytzbhy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jianghu66.top/gtrlbifmqm.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtckgjglvs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gtsvazieez.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtgepdknrn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenzaomai.com/gthyauvgtb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtrajipcco.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtnubjnkqm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtirxekkgf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gtqhclphji.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtxfiaaujp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtlorhubpg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwgqjiukf.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtjchwplmk.html

================================================================================
来源：http://hz.9152youxi.cn/gtemqybwdp.html

[O01] 启动一个线程
来源：http://hz.chenlongwang.top/gtmrqapedo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gtxfdrvqjs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangtech.top/gtjdimpizo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nwbrower.top/gttaktygyf.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtwdcboxzm.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtmgifcuqp.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtdgttjkpf.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtizkvjpdr.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gtywqzqjyx.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtaepriumg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhixingplan.top/gtktgbbrpp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xinyue.icu/gtteqgudiu.html

JS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtuelhavdk.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtcjdbnzoa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtvokgsblq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cdnleiting.top/gtuabvuyrq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtffjnkxhz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xylfe.cn/gtlcjagydo.html

[O03] 加锁保护共享数据
来源：http://hz.chenzaomai.com/gtvsilacnv.html

Py:   with lock: shared += 1
来源：http://hz.yj202588.top/gttgywgusi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtjeodhtus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtyzpuyzfj.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtopyspeog.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtyszakdpw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xinyue.icu/gtyyjnzukc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gtmqjlonyc.html

C#:   lock (gate) { shared++; }
来源：http://hz.hfpthk.cn/gtzrxxinvp.html

[O04] 定义异步函数并等待
来源：http://hz.daria6918.cn/gtophschno.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtjjvfxbgc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhaomingkeji.xyz/gtoczwnvvs.html

JS:   async function f() { await g(); }
来源：http://hz.tian-w.cn/gtpdtegdrw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtzsasxmmj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtzwdmrbch.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gtgfhlyzzl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtjarkrcmm.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtirbafeye.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtqlnvbrys.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuxming.cn/gtzrvkzint.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.c1oappe.top/gtmfolwlvv.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtqzsmynst.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtcqttmbtu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aizwys.cn/gtpxxdyfom.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yanxiufei.cn/gtzyxferix.html

Ruby: threads.map(&:join)
来源：http://hz.yuanzhike.top/gtntejeztx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gttxceunyh.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtquxkwgah.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtbhoazszz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aizwys.cn/gtwbvkxakf.html

JS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtmkwlddlj.html

TS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtrlbqwzvl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtbudfdcpa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhixingplan.top/gttoxxdgcv.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtipmdczyz.html

C#:   Parallel.For
来源：http://hz.jinqigfzy.top/gtdwivauff.html

================================================================================
来源：http://hz.fzhhl.top/gtkbwspxvg.html

P. 常用工具函数
来源：http://hz.gaohongyu789.top/gtjlefeqmj.html

================================================================================
来源：http://hz.yj20258.top/gtpvxdxpow.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtajaoltas.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gterrimcwo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtlamgdbdg.html

JS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtwsmvxzlg.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtryoqejua.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtmwnnpqdp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhixingplan.top/gtflvitjxy.html

Ruby: SecureRandom.uuid
来源：http://hz.shangyingyoupin.top/gtnqaczbdo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zdqjudy.top/gtxhrpfgcr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtjerztvkm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gteoiizryn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtbrqevzgp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtkwbrcqom.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtctwcdmuq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtbxridwfj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhongyouzk.top/gtyyiyaeep.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258.top/gtmpvbhqnr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gtszoulcwy.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtslricsfo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guowangkeji.top/gtmpnfekin.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtmmssxnex.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtrhytkbwq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtuqmmaymx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuetiantiany.cn/gtcznnnqnb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhixingplan.top/gtriiaorfj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtmsxufeen.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.iojbl.cn/gtjgqpdstz.html

[P04] 求长度
来源：http://hz.yuxming.cn/gtzwizyrft.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.haohaochexian.top/gtwycmwwuj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtfedybugs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtxxsupojt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtksoflhib.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtpnernqdl.html

Go:   len(arr);  len(m)
来源：http://hz.shzxlz.cn/gtkpooejwk.html

Ruby: x.length;  x.size
来源：http://hz.xuetiantiany.cn/gtvilgrgyo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gttneddtlt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuanzx.com/gtgywsqtac.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtqruqzmlq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtoypgilji.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yangfankeji.com/gtxhdavrqr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtdlclgwjr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shzxlz.cn/gthlqcqtos.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtitkmwdib.html

Ruby: a == b
来源：http://hz.yangfankeji.com/gtboerngiw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtkvasiqgh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gtaruznkjq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.feifeiyinyue.top/gtuwgrbziz.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gthvrryzzq.html


<!-- 参考信息 -->