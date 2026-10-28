代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtwqczqmdm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtboewkqpl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtobzyusri.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydzc1.top/gtmhuqldjf.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtiovxhgov.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtebydsbpj.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtgavquedr.html

JS:   process.cwd()
来源：http://hz.bjfxy.top/gtperyhnvc.html

TS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtocaqvtaa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtxtieykow.html

Go:   os.Getwd()
来源：http://hz.dashuyun.cn/gthfewtmwk.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtcwxpfpda.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jlsjyb.cn/gtwgjbyfxi.html

[M05] 设置退出码
来源：http://hz.316326.xyz/gtnticmodm.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtyrbsdwtm.html

PHP:  exit(1);
来源：http://hz.smart0.xyz/gtexcltvzr.html

JS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtxlxgitgg.html

TS:   process.exit(1)
来源：http://hz.zdqjudy.top/gthwkdgnqn.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gtpbhklgud.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gtddxwyehf.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtjnmrewrt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtivnatvbu.html

[M06] 向标准错误输出
来源：http://hz.nanxuanxn.top/gtszbwnriq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtzregbkvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.mhx1999.top/gtexmbvfgs.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtreemamdl.html

TS:   console.error("err")
来源：http://hz.ydzc1.top/gtqzqxcrje.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtsewzlahe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtjkdulrml.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtasnvisft.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtlcflwuat.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtficxrqjl.html

Py:   if __name__ == "__main__":
来源：http://hz.pycfn.com/gtrkpdgift.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtiudsnegy.html

JS:   require.main === module
来源：http://hz.havefunace.top/gthmffiqrj.html

TS:   require.main === module
来源：http://hz.hfpthk.cn/gtuqkutoyo.html

Java: public static void main(String[] args)
来源：http://hz.iojbl.cn/gttdtmhjnj.html

Go:   func main()
来源：http://hz.zhongyouzk.top/gtisjrhmpu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hywenlv.cn/gtujrfocwa.html

C#:   static void Main(string[] args)
来源：http://hz.hammf.cn/gtrupaozef.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtsuouknim.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigufen.top/gtznupplot.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtycqcncbt.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtkyljklmz.html

TS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtlitsrmlg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtyurvvfxv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zdqjudy.top/gtlmpryxdg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtibmydwhx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yueranfly.top/gtvfpnqtsh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvpqqeymp.html

N. 数据结构与算法
来源：http://hz.andypj.xyz/gtquwcjhfw.html

================================================================================
来源：http://hz.cheryme.top/gtbtukcopp.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtuffhcfab.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtwdihoszk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtfuykbgrj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtkztabptc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtbryigywv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yonumen.top/gtelbqaual.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guowangkeji.top/gthpgifxjc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtmbplocyf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtdscrvksi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ywan-chungtsiang.top/gtqawngwui.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtrtvxxqhp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gtzijyvnci.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtvlkhrhrs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtqgzjsyfk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gttgapxnmh.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtwrxttcka.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtuskijbcf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtdfqomkxs.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtbolkqexg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gttqbfxvfh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtusawnlun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtllvxjdqv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtsybqrxts.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.316326.xyz/gtgjcbizhz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtrezszgyi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tianlin.xyz/gtppzbnqrh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtilutpkpc.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtnrobgqdd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gthwcahxim.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtzxxokkau.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtmfradprm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtykuwnavi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhongyouzk.top/gtjhnllciy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtelyxsglq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtanakrnna.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gtrorhpyop.html

[N05] 最大公约数
来源：http://hz.shangyingyoupin.top/gtoaqrxfgh.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtxoczwbrc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guowangkeji.top/gtrojzhcao.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtvinnggmd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtdonkczei.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gtmxdnoxpc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.9152youxi.cn/gtykqsminh.html

Ruby: a.gcd(b)
来源：http://hz.redwolf501.top/gtglujgsna.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtfrjmudre.html

[N06] 判断回文字符串
来源：http://hz.gotoacloud.top/gtgmzmyzki.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtqywucxjz.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtsarxirdl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtfdkpcryl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gttwpzjrui.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtoahvfdey.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtdtjcgpyx.html

Ruby: s == s.reverse
来源：http://hz.daria6918.cn/gtednymvzc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guannengcc.top/gtfscadyhg.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtmidszcij.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtohtnlwhr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yanxiufei.cn/gtkwmihizl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuanzhike.top/gtgcnxfhjx.html

TS:   // 手写 Map<string, number>
来源：http://hz.cdnleiting.top/gtxamchhqh.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtfycfdgdq.html

Go:   // 手写 map[int]int
来源：http://hz.havefunace.top/gtqaoexhod.html

Ruby: // 手写 Hash
来源：http://hz.jqgfzy.top/gtnrylaztz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gaohongyu789.top/gtscjepefa.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtbyfldxrh.html

Py:   itertools.permutations(arr)
来源：http://hz.zycfv.cn/gtgrsoyivp.html

PHP:  // 手写递归交换
来源：http://hz.pengpengdd.cyou/gtvofuhdnx.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtzuehlvww.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtzfasrshr.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gthcyzkrhv.html

Go:   // 手写回溯递归
来源：http://hz.yj202588.top/gtkpbfajlr.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtbhvdjglu.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtfrbhnjpo.html

[N09] 栈与队列
来源：http://hz.cdnleiting.top/gtbzcdtyyj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cdnleiting.top/gtxuepubsn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtcvgxcvfu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gtgnqsasqq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhongyouzk.top/gtnhlvlbhz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigfzy.top/gtixmyfmas.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtcqdvmdcz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtvuotvaxb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtqnljtnnx.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtmomzltap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtfsoqdxiw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pycfn.com/gtenwdlyyh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhongyouzk.top/gtwvanswbg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtzfmmlkmu.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtgdeszcul.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sysykeji.top/gtwighljwa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gttngnqfsn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.smart0.xyz/gtmvvyuiof.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtmdufvtjs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yvedp.cn/gtlasexkmn.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtroeumxcq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtrhcissfx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtypdbfnrb.html

Java: // 手写递归
来源：http://hz.daxiang520.top/gtybvozvqh.html

Go:   // 手写递归
来源：http://hz.yangfankeji.com/gtszcgduyq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtlhmqvbjo.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtbxczpzab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtxkerjwph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gtljvidwya.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtbkypxrgz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtverdzimk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtgigwcfdb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gttrxjjbjt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtpstfgcln.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gtywmrcorr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtyggexwac.html

================================================================================
来源：http://hz.pycfn.com/gtkufrwkhd.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtuvdmzoxn.html

================================================================================
来源：http://hz.yj20258888.top/gtvbjecnvi.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtebrumsrw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gtdrpvhwxs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtvdrxkchq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtuxunjwuu.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtdvornkky.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtcqyyiola.html

Go:   go f()
来源：http://hz.yuxming.cn/gtqqpplxqd.html

Ruby: Thread.new { f }
来源：http://hz.jiagoushi.top/gthacoclik.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtxbzzfrqf.html

[O02] 使用线程池
来源：http://hz.zhiwuduotai.top/gtoypxhaqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dashuyun.cn/gtepjdtsrn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gthjopsegd.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtbrzncaib.html

TS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtonaprwhg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.redwolf501.top/gtznzbqxix.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenlongwang.top/gtnpuqoyap.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtvxirnjjp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gttuhziwzh.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gtxxyngmjz.html

Py:   with lock: shared += 1
来源：http://hz.jqgfzy.top/gtugtmzltk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigfzy.top/gtoibsanqp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtafoxqkkg.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtnktcongo.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtspehsizi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxinkj.top/gtpetcaluk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtfivtjxyj.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtojlhmlfh.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtxurxrixe.html

Py:   async def f():⏎    await g()
来源：http://hz.316326.xyz/gtoritykbo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.vqdsnc.cn/gtrrehdfxm.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtdckdpkvp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtrsziwntw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.0kj1m.cn/gtexkkcxjn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cqqwz.cn/gtzisxcnaa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtflpdaisw.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtidvhzjvs.html

[O05] 并发执行并等待全部完成
来源：http://hz.andypj.xyz/gtripcruah.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dashuyun.cn/gtyjfkphta.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gtakfuriwb.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtazqkkmjh.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtqzzdvhaz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtfufcovse.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gtvjnzdrfu.html

Ruby: threads.map(&:join)
来源：http://hz.hammf.cn/gtvyrxwkot.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtjkyquumj.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtsltdnwul.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guannengcc.top/gtircfiiot.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shangyingyoupin.top/gtkjscyldu.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtuszazslu.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtcktjkzrs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.kuanghao11.cn/gtwetpukak.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangkeji.top/gthyvprjdt.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtegjltxtt.html

C#:   Parallel.For
来源：http://hz.daxiang520.top/gthucubcah.html

================================================================================
来源：http://hz.svipenyu.cn/gtgrwlymnr.html

P. 常用工具函数
来源：http://hz.svipenyu.cn/gtoeidwbsk.html

================================================================================
来源：http://hz.gogol.net.cn/gtusaagdvu.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtnfygnwyc.html

Py:   str(uuid.uuid4())
来源：http://hz.havefunace.top/gtqyzhjlbc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aizwys.cn/gtzckytgwy.html

JS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtivimrkpt.html

TS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtfalztxvu.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258888.top/gtjodeeocv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.havefunace.top/gtytxstoaz.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gtkamlsiyc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xingfuxueyuan.xyz/gtdxoeqhkj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtcyghwvwz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtoyxepere.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxuanxn.top/gtkhzpeijx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guannengcc.top/gtgexcbeyg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daria6918.cn/gtdfypjevd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gtcqtqskal.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtrhqueitv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtqckabuiw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xylfe.cn/gtbdbddvse.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtgicroupn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yonumen.top/gtwabfjjon.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sysykeji.top/gtgxodtovb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtmgbfsavb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtmnjusadc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jyoumei.cn/gtccyfrtuc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hfpthk.cn/gtnhjcunsu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hammf.cn/gtkimkokgx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xziqi.cn/gtwnrrfajt.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtmbvbjkgy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinyuanbaomall.cn/gtzgowqsjs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtoxgntnsq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtlafofvld.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtxwkgscov.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gttlzzvbkw.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtnbgmrucm.html

Ruby: x.length;  x.size
来源：http://hz.yj202588.top/gtzgqlcnmg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pengpengdd.cyou/gtnjyltxdc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gthivvybuk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtbrmgyeif.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtdmytkzut.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtofwxfpmi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtnhzfpnxe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtaudtkulw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtwjissxzr.html

Ruby: a == b
来源：http://hz.guannengcc.top/gtdlpwzoyv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtqmadudaa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtboctmbjo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtdlnspank.html

PHP:  if (empty($x)) {}
来源：http://hz.zhixingplan.top/gtevkgwkhh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.birdmap.top/gtadfzagvq.html

TS:   if (x == null) {}
来源：http://hz.ivvv.top/gtdgtfkayi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtjtvjumyh.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtlgnxguhf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gogol.net.cn/gtwumqbrvd.html

C#:   if (x is null) {}
来源：http://hz.redwolf501.top/gtnttuxasu.html

[P07] 防抖与节流
来源：http://hz.ydjk.org.cn/gtfscdjgai.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtbvleamcq.html

PHP:  // 手写时间戳比较
来源：http://hz.xinyue.icu/gtwspcgjoh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtuwdtiywl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gttabwftmy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinghuilouyu.cn/gtpqnrzrkx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sysykeji.top/gtdyhfmlrf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtvdqrjwke.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtyrezcvsw.html

[P08] 处理浮点精度问题
来源：http://hz.haohaochexian.top/gtmwpqyyoa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ybcxt.top/gtxmrnssxo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtifiadmip.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtowcjjamj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtapfyxkwg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gtvrwgigbw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gteoxukxbc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gtvnkzsvwf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtcfjtrzqo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtnmtyljkc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinyuanbaomall.cn/gtfrkaifzu.html

================================================================================
来源：http://hz.sufxvd.cn/gtcnnoxhdo.html

[Q01] 创建表
来源：http://hz.chenlongwang.top/gtcsmwdyjc.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtmnyjqwhw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtaiklxvaa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtpahkuteb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gtxthgtmdh.html


<!-- 参考信息 -->