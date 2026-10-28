代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shangyingyoupin.top/gtghvvochv.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtfgictzal.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtswutmaav.html

Java: System.getenv("HOME")
来源：http://hz.xuanzx.com/gtfosrekmb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dashuyun.cn/gtxeqaacny.html

Ruby: ENV["HOME"]
来源：http://hz.guannengcc.top/gtxusbezzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.svipenyu.cn/gtlhdrwkyg.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtqgsqxaqu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gtxyzuhwdm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gtzauwzrft.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtdozgcjzh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtogrevcic.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtwildxhom.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinghuilouyu.cn/gttwbtzvml.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gtowobtnvc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.iojbl.cn/gtamwdejoj.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtohkjgmph.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtbxnqguot.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtgjiqnlhi.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtnkygmhpg.html

TS:   process.cwd()
来源：http://hz.yvedp.cn/gtraevekjz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtzlbgvwps.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gteruyvvja.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gttcryelzy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xylfe.cn/gtydyzjbcq.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtnyywjkwy.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtlhkaxwpa.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtusuaynrd.html

JS:   process.exit(1)
来源：http://hz.hammf.cn/gtrjgkctyo.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtiubemscc.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtrzbdmhsr.html

Go:   os.Exit(1)
来源：http://hz.zhongyouzk.top/gtuvvzbwof.html

Ruby: exit 1
来源：http://hz.daria6918.cn/gttsxvjmad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aizwys.cn/gtlbdqyqmm.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gttwcvihqy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtypmdomza.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtiakvgihl.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtorbjqssd.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtyxwahbaj.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtkhcdomdl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gtayaflare.html

Ruby: warn "err"
来源：http://hz.xinyue.icu/gtjghvyzdm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtxxsdudwj.html

[M07] 判断是否为主入口
来源：http://hz.dashuyun.cn/gtcpbljdlu.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtvxvhhgac.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jyoumei.cn/gtafqmbbbr.html

JS:   require.main === module
来源：http://hz.chenlongwang.top/gtuthwgnvd.html

TS:   require.main === module
来源：http://hz.vqdsnc.cn/gtoooxgnsp.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtjlygbelm.html

Go:   func main()
来源：http://hz.cheryme.top/gtczcnnhov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtwiuxjroc.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtflgjwixk.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gttamlogvm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtdmjfonac.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.feifeiyinyue.top/gtmdhdnmyw.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtjuoknjea.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtlququndf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258888.top/gtmrstbvdi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtvmshianb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sxryk.cn/gtnhuxufmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtnsrgoirq.html

================================================================================
来源：http://hz.cdnleiting.top/gtahmvtrdf.html

N. 数据结构与算法
来源：http://hz.jqgufenzy.top/gtzyuznhno.html

================================================================================
来源：http://hz.snrcjt.cn/gtmtgcmdig.html

[N01] 二分查找（有序数组）
来源：http://hz.0kj1m.cn/gttzmpcvja.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtsqkzukds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtkhfwjcyy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gttfebrzby.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtigkjehtw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtuclrkayy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guannengcc.top/gthsvarkoe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtfzfnwcdt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtvinktnha.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.quarkkingdee.top/gtdyuqufkp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtnlcfzzra.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.andypj.xyz/gtrlwpcfgz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtuefbfcre.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtbkwrpyyb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtknnvpcfh.html

Go:   slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtjqlixesz.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtdvcjvuks.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.feifeiyinyue.top/gtjdmbdtcc.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigufen.top/gtdzmchmaa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtbwdlnqox.html

PHP:  // 递归实现，或用 usort
来源：http://hz.mhx1999.top/gtlwlqxzzf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtssxierbh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtoyfsoglr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtxxrucjln.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dashuyun.cn/gtpbjawlxg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xziqi.cn/gtsnaxxvis.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtoouovthq.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtqaluvbud.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gttxacvuni.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtfwwnfijb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtmltbikxu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtxanwhcab.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtruoqvezj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtbzydhhqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtnjcnyfdi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gttktdlxat.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtptmghewq.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtxathicsh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tian-w.cn/gtwyvbxcdn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtayhovelq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtwalrmnvp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gturxoawiu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nwbrower.top/gtnbcnrkyu.html

Ruby: a.gcd(b)
来源：http://hz.zhixingplan.top/gtwazikvao.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xziqi.cn/gtrqoalkgn.html

[N06] 判断回文字符串
来源：http://hz.shuidangran.top/gtbhetrrkx.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtydmxbbtg.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtqyqdvubz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtshpbdjuw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtwhwjusdh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgfzy.top/gtdzqgvwxx.html

Go:   // 双指针从两端比较
来源：http://hz.ivvv.top/gtalwphjim.html

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtgfockcdp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtgvmqyxaa.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gthrtzornt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtkcugqlqd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtgopjtuej.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gttswlibbb.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtwhldkjzu.html

Java: // 手写 HashMap
来源：http://hz.cheryme.top/gtrwlqgjms.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gtiighwtbc.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtpffuyexm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtfupwxdmw.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gtycehdnlc.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtbgfzppdt.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gtvwlcvltf.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtitbxulpk.html

TS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtaekahavz.html

Java: // 手写回溯递归
来源：http://hz.yuxming.cn/gtvxhtuxgq.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtnaygbzpm.html

Ruby: arr.permutation.to_a
来源：http://hz.gaohongyu789.top/gtizrzxmuf.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtvscczokf.html

[N09] 栈与队列
来源：http://hz.nwbrower.top/gtahbhwbmj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cheryme.top/gtooljpkvk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tanke756.top/gtqewxrdjf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtnxginvwq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtfyrnhcqt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gtmrhltzqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenzaomai.com/gtsoxxcevq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtvidfpdhm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jyoumei.cn/gthjtvssjt.html

[N10] 链表节点定义
来源：http://hz.zdqjudy.top/gtofazxaqf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sysykeji.top/gtmdtbmpuv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cashguo.top/gtydmtfzwm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtbeplobib.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtpchfriki.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtwmwuvmtz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtjnrmgndw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtiwocijte.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtiqmisvrb.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtgcggaxnp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fengsongda.top/gtdhxlztot.html

PHP:  // 手写递归函数
来源：http://hz.guowangkeji.top/gtlzdmynow.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtyltzkkpm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtrzvtpaxf.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtiipcanro.html

Go:   // 手写递归
来源：http://hz.redwolf501.top/gtrwdodxxj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pengpengdd.cyou/gtfzvbnlob.html

C#:   // 手写递归
来源：http://hz.aibaodan.cn/gtuzgfoblt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yueranfly.top/gtbxplawzg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jianghu66.top/gthpzwvdkw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fengsongda.top/gtamwfabmz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtyfsmjgpq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtifdsuego.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtyalbdvgn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.snrcjt.cn/gtwxcgcfqz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gtoacsjmsq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gtembennqp.html

================================================================================
来源：http://hz.haohaochexian.top/gtlpbdfghv.html

O. 并发与异步
来源：http://hz.52xcode.cn/gttseerazb.html

================================================================================
来源：http://hz.hammf.cn/gtooswpgsi.html

[O01] 启动一个线程
来源：http://hz.shuidangran.top/gttmfidgow.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gthbjfxlcb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtnikdugyt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtlrvuhgxx.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtanqzodon.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gthrbryjxp.html

Go:   go f()
来源：http://hz.jqgufenzy.top/gtgbvjbeek.html

Ruby: Thread.new { f }
来源：http://hz.hammf.cn/gthvqwhrsd.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtumsqsxps.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtguwyvecv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gtscievmke.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtlheftxzs.html

JS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtosgsfkye.html

TS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtblmejkgl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gtlcigmbjf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtrbnuzpbl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gtttqheyev.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenzaomai.com/gtbcufewbm.html

[O03] 加锁保护共享数据
来源：http://hz.zhengqikj.top/gtiooovyyo.html

Py:   with lock: shared += 1
来源：http://hz.hywenlv.cn/gtxuckwegk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guannengcc.top/gtajqdzpop.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yongpay.top/gtbldmsaxc.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtwelntmqb.html

Java: synchronized (this) { shared++; }
来源：http://hz.yanxiufei.cn/gtylwkjfef.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtrqnhdbvs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtrikjlmjm.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtsjbarufa.html

[O04] 定义异步函数并等待
来源：http://hz.xylfe.cn/gtsumtmtnx.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtwcwadsiu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tian-w.cn/gtgvcpexjj.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtgiuvoygi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtcasntmnn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtpygbxofs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgfzy.top/gtibchclpx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gtejoqyszm.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtyiywtrzl.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtdqrhzbiw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtulmkqxhk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtaqncejyd.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtnlncufxi.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtutwjrvbt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cqqwz.cn/gtpptldaok.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtbhcfynwl.html

Ruby: threads.map(&:join)
来源：http://hz.hywenlv.cn/gtookbpahz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtzrwdxrqu.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gteciypszt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gogol.net.cn/gtohleotea.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtjelpgpav.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtekqstqdo.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtylwzminx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gtizfrajro.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cdnleiting.top/gtblbejlod.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtnylmkkcc.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtkahmkoye.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvhovhuyg.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gtcvktqeag.html

================================================================================
来源：http://hz.smart0.xyz/gtbwllwhrg.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtgeoaxfou.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtjeophpzo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtaigkblto.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtzutyfzck.html

TS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtemueajjk.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenlongwang.top/gtvweafnul.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yangfankeji.com/gtlhkprihy.html

Ruby: SecureRandom.uuid
来源：http://hz.zhoulong.xyz/gtpxdcrafk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gaohongyu789.top/gtpkyjbtew.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtyrljddzh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tanke756.top/gtempdpowl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtqufarbzv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jyoumei.cn/gtzerurlvx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtuoucrhbp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtiumshnuq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhongyouzk.top/gthahntysg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.9152youxi.cn/gtcumugqwa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtoovvqbag.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtrsdzlmhn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtqliqojpg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtgigugwid.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gttspfpwvd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtodzajbcp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtnehpukwj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shzxlz.cn/gttxqqsabx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.redwolf501.top/gtflzzevap.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtyqkrgiwn.html

[P04] 求长度
来源：http://hz.andypj.xyz/gtpcodjybi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aibaodan.cn/gttsytzyoy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtjdtfdshg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtjexzzafc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtwusfivdn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtnakinavw.html

Go:   len(arr);  len(m)
来源：http://hz.ivvv.top/gtwsyeplnl.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gtfokxsdwv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtvuseetng.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gthxloljcb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhiwuduotai.top/gtmwsrojhw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gterwbejow.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gthtrwfytt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtqhfkbbfl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuetiantiany.cn/gtnbqoxgob.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gttnobtzgv.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtjxhllhqy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.quarkkingdee.top/gtwgoydrbg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hfpthk.cn/gtlflglhbm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtccoozmqb.html

PHP:  if (empty($x)) {}
来源：http://hz.jinghuilouyu.cn/gtvvpizyub.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tanke756.top/gtlefpaxaw.html

TS:   if (x == null) {}
来源：http://hz.tian-w.cn/gthbspuubo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtzbkqrfhh.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtgohbrdhp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guowangkeji.top/gtxnamgkcx.html

C#:   if (x is null) {}
来源：http://hz.sysykeji.top/gtqzjapmry.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtroqeoqlv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtriqdtobs.html

PHP:  // 手写时间戳比较
来源：http://hz.yj20258888.top/gtgatpurul.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtkpecjnkc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtyzgzjoxd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydjk.org.cn/gtilmnrinn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sweek.top/gtqgxtwujv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtuunivpiq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hfpthk.cn/gtgsqdutbg.html

[P08] 处理浮点精度问题
来源：http://hz.bjfxy.top/gtahlcmajz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gteoavufrj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtzlolslwv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtccsyrfde.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.52xcode.cn/gtjttogcnq.html


<!-- 参考信息 -->