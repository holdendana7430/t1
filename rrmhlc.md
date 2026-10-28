代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtnaaostjp.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtkafyhwrf.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtcboqcune.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtcymxqfvl.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtejyiormt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtlaqwpiap.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gtohbwxvso.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtsmcnlgyd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtqjnvudav.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtfxyoazfu.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtanqjitmj.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtjsoxshvd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.quarkkingdee.top/gtardrwnnu.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtmyhfowsb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gthggeubuh.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtqpaecxju.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtoumvrkuh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtjkzsfhmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtpnoldhla.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtobxgelie.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.vqdsnc.cn/gtquvqsppg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgfzy.top/gthmlhicda.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.quarkkingdee.top/gtbidveyck.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtczrwodfb.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtnkfzersy.html

Py:   os.getcwd()
来源：http://hz.ivvv.top/gtnidijcfq.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtfgsolzck.html

JS:   process.cwd()
来源：http://hz.yonumen.top/gtuqzgvodt.html

TS:   process.cwd()
来源：http://hz.hywenlv.cn/gtdfgyyzhl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigufen.top/gtgxocbdbz.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtayuiobpc.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtyudsoyou.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtbbikiron.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtyatlarmo.html

Py:   sys.exit(1)
来源：http://hz.yuxming.cn/gtqahtpxwr.html

PHP:  exit(1);
来源：http://hz.cashguo.top/gtweidcomh.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtnebzrwzg.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gttistkmeq.html

Java: System.exit(1)
来源：http://hz.iojbl.cn/gtplbeizuq.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtmkjoryyq.html

Ruby: exit 1
来源：http://hz.316326.xyz/gtqjdwgrxv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gttuemkues.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gttiljbnqb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtjyqmdxtv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtmxmiboia.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtwudmross.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtrimvouax.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtpyridoie.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtlxsxgumi.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gtrorckbls.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtfexbclcq.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gtexqisptt.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gteyaqqqvg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtjvdgqysz.html

JS:   require.main === module
来源：http://hz.ehwqpu.com/gtpwprtkiu.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtxljnvkzx.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtioseztpt.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtfqajybhi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtzynqjcph.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtfbxsolii.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gtgielzljm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtidtbpymp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangkeji.top/gtvkldrbza.html

JS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtxjdrunsf.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtfskxeyns.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.birdmap.top/gtwfdpetjp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtcvreiqfj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cdnleiting.top/gtkviwhjrf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtdxtsnwwd.html

================================================================================
来源：http://hz.nanxinkj.top/gtyexcgagp.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtghdoxcqj.html

================================================================================
来源：http://hz.svipenyu.cn/gtugufpapu.html

[N01] 二分查找（有序数组）
来源：http://hz.meibo888.top/gttocddlsb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gteapplrlr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shangyingyoupin.top/gtcxkrfimi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtxjcrzgiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtyimdbwje.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yueranfly.top/gttotcikbc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtqcjbdsyo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtewpfmhyn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtqjcguxng.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtoyjgefwo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtpdxjgqdy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtemhtcfeu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtxinfuxzi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtdacjhcbo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gotoacloud.top/gttznqntcr.html

Go:   slices.Sort(arr)
来源：http://hz.guannengcc.top/gtvlwvksem.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtclihoztx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtkckruanc.html

[N03] 快速排序（分治示例）
来源：http://hz.andypj.xyz/gtaxykmeev.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtkqifnban.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fzhhl.top/gtovmecqcc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtjsgabvji.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gthrmajasm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gaohongyu789.top/gtfpahmxuq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtaitxdvsx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tanke756.top/gtrygzqrsy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gtnkvnrlhq.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtkhtwdplv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtdejpldkx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtdssnxnza.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtdhgwkmuz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtumekzluf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.mhx1999.top/gtriymifqe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtfvtroysh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtydaxnfkb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gtulhmjcbd.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtnofmadlx.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangtech.top/gtdvlmdwdx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gtietcifbq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gttrdugmdb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtjznzobmy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtrsazmouo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xylfe.cn/gtztxxzycf.html

Ruby: a.gcd(b)
来源：http://hz.bjfxy.top/gtnubwpopu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtcqktdxue.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtpzzgepla.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtofnsptof.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtppuisiqm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtzclqogii.html

TS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtpsrnlbtg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtawdwltps.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258.top/gtboorxqiu.html

Ruby: s == s.reverse
来源：http://hz.yj202588.top/gtpavflncn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtguoiukui.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gtrsqjrdms.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daxiang520.top/gtnnduiyzm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.kuanghao11.cn/gtoqejugxa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtkbqrfrsh.html

TS:   // 手写 Map<string, number>
来源：http://hz.guowangkeji.top/gtdbtoqkix.html

Java: // 手写 HashMap
来源：http://hz.jlsjyb.cn/gtddvtpchi.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gticrsiywv.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtkbqzrrwh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtseozkktt.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtdcukubpu.html

Py:   itertools.permutations(arr)
来源：http://hz.jinghuilouyu.cn/gtpvkcjlci.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtwaifnmbg.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtdvjnzpeg.html

TS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtciyeyjuv.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtwkjfvuxg.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gttbkmiaca.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgufenzy.top/gtpqvvagqi.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gthceatgay.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtyednuoxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtvxyujprg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtbfxpyloy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtjrdhyhon.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.c1oappe.top/gtjlleiuaf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gtnggwuoyu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinghuilouyu.cn/gtlafhaxmd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtpdxztpzv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenlongwang.top/gtxzzqwibo.html

[N10] 链表节点定义
来源：http://hz.snrcjt.cn/gtkuyofbtp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gteyayljql.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hywenlv.cn/gtwcmwhomr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gtotxvtgvg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtalcomnsb.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxuanxn.top/gtcxgmgjzf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gttdjunzeg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtpiwtikxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtmkkwsvpp.html

[N11] 二叉树中序遍历
来源：http://hz.jlsjyb.cn/gtodbgrizz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtrclttyqu.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gtxmuxnkqh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtqdkvzmbm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtvrgzgors.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtdtmqfvlm.html

Go:   // 手写递归
来源：http://hz.jinqigfzy.top/gtsjcaruvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtonumzuqh.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtwfddytxs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ybcxt.top/gtcyfeglbt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtenkdmzbt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtclwvzctg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtbcioizgj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gteeavnvex.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtybqdzukn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gtbvhhlsck.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gtljmrmowu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtchniatks.html

================================================================================
来源：http://hz.ppjwa.cn/gtkinarico.html

O. 并发与异步
来源：http://hz.redwolf501.top/gttvuufdbl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdgzxejxf.html

[O01] 启动一个线程
来源：http://hz.guannengcc.top/gtxavzbhto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zdqjudy.top/gthfbqupkd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtwlhkftlr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtbzemqzwt.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtgfmnmuqj.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtzhdtoubu.html

Go:   go f()
来源：http://hz.cashguo.top/gtifikogsd.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gtictoslov.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtmehndfir.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gtjawiicka.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ehwqpu.com/gtlaabqzqt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gtttmcddsc.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtqfosbutv.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtzkaqdebx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtaqvubpvg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cdnleiting.top/gtteykyrrp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtuhymjuaf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtxuttxors.html

[O03] 加锁保护共享数据
来源：http://hz.zycfv.cn/gtkcryffqw.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtrmtqsiiu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhixingplan.top/gtoumzasuu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gtjzbdcgxb.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtfelnwiij.html

Java: synchronized (this) { shared++; }
来源：http://hz.gogol.net.cn/gtmhliengd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sxryk.cn/gtrditfopp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shangyingyoupin.top/gtxtytlpmj.html

C#:   lock (gate) { shared++; }
来源：http://hz.shangyingyoupin.top/gtbfbyemun.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtulhxfwcc.html

Py:   async def f():⏎    await g()
来源：http://hz.xingfuxueyuan.xyz/gtobumzhoe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtqjrpuibn.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtnzhpgnyd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtgfpfllir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tanke756.top/gtojfidelu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gtjjgvqhve.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cdnleiting.top/gthhmmcrvz.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtejbhxtxt.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gthvazxret.html

Py:   asyncio.gather(*tasks)
来源：http://hz.andypj.xyz/gttmvsnrwf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgufenzy.top/gtbyoweymu.html

JS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtfdjmpksi.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtoaicvkdy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtqcsjeokz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxuanxn.top/gtorfrxbnh.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtavibahth.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.9152youxi.cn/gtouqfelsc.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtrtrwlwfv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtzmhhgnmw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gthghxiroz.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtuogsizav.html

TS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtljncqgzw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhaomingkeji.xyz/gtfdpocihl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtdwgcanan.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtmjukrhit.html

C#:   Parallel.For
来源：http://hz.0kj1m.cn/gthllgwduy.html

================================================================================
来源：http://hz.cucudq.cn/gtxnhloqsk.html

P. 常用工具函数
来源：http://hz.ybcxt.top/gtooqnikje.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthibmsjku.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtqfioyzqz.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtldmxckpw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.svipenyu.cn/gtuwegdmnw.html

JS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gttunnbwvj.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtrvxekmjh.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gtlousshom.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pengpengdd.cyou/gtjzvqigdf.html

Ruby: SecureRandom.uuid
来源：http://hz.zhixingplan.top/gtijllssvt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gtwroenvls.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtnqyvdgqc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pengpengdd.cyou/gtcodtxtrf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yonumen.top/gtimfuyxyv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtnbsxlvez.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtjsnougwe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtfpctvfmv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ppjwa.cn/gtkulkidiy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtzjoaskez.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtryrwzzgn.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtxpcbrzqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnxiangtu.top/gtytvleyhe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sweek.top/gtasjuohzd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtynasknxz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtdvpeqaba.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pycfn.com/gtllwnrqxm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jianghu66.top/gtbtbwmwuc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yueranfly.top/gtdcxyhuud.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.kuanghao11.cn/gtcvyngbsf.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtagbpjlif.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.haohaochexian.top/gtjnwwxzec.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gttfegnhux.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtuuekxicn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtickluvbd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.feifeiyinyue.top/gtlbipfkkj.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gttppviwri.html

Ruby: x.length;  x.size
来源：http://hz.tian-w.cn/gttdowqcjk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtbgmpwsgd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinghuilouyu.cn/gtxozloclz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtbdcaormz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtlhrwisvx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtrdiisiwl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gteixiygyw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtunpqypka.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.316326.xyz/gttnsghwxr.html

Ruby: a == b
来源：http://hz.nanxuanxn.top/gtuvrjoylb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtoyiszytu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtumsqorkf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtlzvrmtgv.html

PHP:  if (empty($x)) {}
来源：http://hz.yangfankeji.com/gtwueiawbo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtnlfzigna.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gtgcltvqqk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daria6918.cn/gtlkfnqloe.html

Go:   if x == nil {}
来源：http://hz.xingfuxueyuan.xyz/gtnuexzvqx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtmrisyuzf.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtatdsvdzf.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtueildsum.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtmaigmuwk.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtougvihfi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtmzrqhsfh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtlzxvxmfo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nwbrower.top/gtxkacjfgz.html


<!-- 参考信息 -->