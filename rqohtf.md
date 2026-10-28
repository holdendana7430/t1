代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtuwlphkwc.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtbvuzlirx.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtsubyuqip.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtalbnxpgh.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtnavckblg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtukwvujka.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtcozdacri.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtfjyemlzs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtukkopqpd.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtkhbfmepr.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtlpegvufs.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtqfjugmkp.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtaaaupafv.html

TS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtcoapmvmk.html

Java: System.exit(1)
来源：http://hz.dashuyun.cn/gtxbmhorua.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gtwrnycqjs.html

Ruby: exit 1
来源：http://hz.zhoulong.xyz/gtencniida.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtiiyxpiii.html

[M06] 向标准错误输出
来源：http://hz.nwbrower.top/gtzdabknwj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.52xcode.cn/gtzmdiolmn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sxryk.cn/gteqhcsowr.html

JS:   console.error("err")
来源：http://hz.chenzaomai.com/gtlnjqfhwe.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtfwxpmdho.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gttmritqnz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtrswgcwbo.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtapeygpqg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.svipenyu.cn/gtahaizpwe.html

[M07] 判断是否为主入口
来源：http://hz.ehwqpu.com/gtvxkcipbt.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gthqqrdakj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtppfxarra.html

JS:   require.main === module
来源：http://hz.jiagoushi.top/gtwizeqwpu.html

TS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtltqwuawb.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtankcwugj.html

Go:   func main()
来源：http://hz.ybcxt.top/gtxhkhatpw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtmzljwfzv.html

C#:   static void Main(string[] args)
来源：http://hz.jianghu66.top/gtfuseitix.html

[M08] 获取系统与运行时信息
来源：http://hz.sufxvd.cn/gtrztnqejg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.bjfxy.top/gtvywgpfjr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fzhhl.top/gtsahugylf.html

JS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gttnrdxolr.html

TS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtdcmllzzt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtfnagkzxm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtbslmivwv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenzaomai.com/gtwnzqdagb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtjflpxqwi.html

================================================================================
来源：http://hz.hfpthk.cn/gtxlksodoj.html

N. 数据结构与算法
来源：http://hz.cashguo.top/gtpcwtsswr.html

================================================================================
来源：http://hz.yuanzhike.top/gticdeognu.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtesrchfwq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jyoumei.cn/gtzsdbhnbz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gtmlwzkfpn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtfthnpgff.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtykklwmry.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gtxgyymnsr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hammf.cn/gtxnruzlpu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtlinwaarv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtdxroblmk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xinyue.icu/gtvvpkwwzr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtaudmmofj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gttdwprjmb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtximlqgca.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtdpczrxfm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtnqgczkrk.html

Go:   slices.Sort(arr)
来源：http://hz.redwolf501.top/gtqdgfccus.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtknrmwhve.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtqaqmxili.html

[N03] 快速排序（分治示例）
来源：http://hz.nwbrower.top/gtnlxlawmb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gthbhvbmhc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtdbycgkmv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gttyjrzfca.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtwelnbdtp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtttfvuomk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtpcopnkjn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.snrcjt.cn/gtrouniusj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yonumen.top/gtvqrjxhad.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtgfcuzvwp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtlzvmtqzj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xylfe.cn/gtxkharcxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtoexdicyy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtdbxxmavo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtspdgyssj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtqawjtuyq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtynzycina.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtwgmznogo.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtotiyltxx.html

Py:   math.gcd(a, b)
来源：http://hz.zhaomingkeji.xyz/gthpawbixx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtorcdqedb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtibycrimv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtwhmbczgd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtvngqzzup.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtyvkcukfd.html

Ruby: a.gcd(b)
来源：http://hz.tian-w.cn/gtgmcbrebh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guannengcc.top/gtyygnacia.html

[N06] 判断回文字符串
来源：http://hz.hammf.cn/gtqqhrszhq.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtwqwsvnhg.html

PHP:  $s === strrev($s);
来源：http://hz.yangfankeji.com/gttypmtzve.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtmejcgcqw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtwemjowek.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.iojbl.cn/gtkrdxpasa.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtklfrfflh.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gtqlmbyqii.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.mhx1999.top/gtcdsocrmw.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtqhoavjmd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtnyzwirjs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtiwpbhnga.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hongshengwenyu.top/gtxykkowee.html

TS:   // 手写 Map<string, number>
来源：http://hz.0kj1m.cn/gtlbszpibg.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtbmkgrcre.html

Go:   // 手写 map[int]int
来源：http://hz.svipenyu.cn/gtbpsttfnl.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtkbfdlmtz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gaohongyu789.top/gtvrzwwfnz.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtjtvmkgin.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gttjwveiww.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtnluabqzq.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtqihylvbb.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gthlgsbxam.html

Java: // 手写回溯递归
来源：http://hz.svipenyu.cn/gteqrxepfs.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtrqsifswt.html

Ruby: arr.permutation.to_a
来源：http://hz.zycfv.cn/gttsptesfl.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtqxnwvntu.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtudlvdbfu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigfzy.top/gtanckpmph.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xinyue.icu/gtmsutawrr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtiwdjxdzj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtoixxgocg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jianghu66.top/gtpnnavywt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.316326.xyz/gtypdgkirw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gtedhjrbcx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hywenlv.cn/gtmjauewvl.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gtpictcrmq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gogol.net.cn/gtoaskabtr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ehwqpu.com/gtfkzhcvxc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.meibo888.top/gtwtzooyro.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtcuocglwk.html

Java: class Node { int v; Node next; }
来源：http://hz.ydjk.org.cn/gtvlmkbqwb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtkndtmawq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtvvxaacuf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtlzpugwit.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtjoyjasyo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtjuaoehpt.html

PHP:  // 手写递归函数
来源：http://hz.9152youxi.cn/gtxaqblpeq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtepniziui.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtbhiinjhd.html

Java: // 手写递归
来源：http://hz.xuetiantiany.cn/gtklcdhiqn.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtvbongwqd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtmlqzfidz.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtmvtthdit.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtjnudughl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtglqxlbtc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtayzgzaap.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtnwxsyyow.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtmewrcwqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtnsvxbzyq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtzxoapsqz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.316326.xyz/gtdnyrkknw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtdalhvcqv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtprldslil.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtrniirrtw.html

================================================================================
来源：http://hz.snrcjt.cn/gtfwjvbpbu.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtaafwibgu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ybcxt.top/gtrpjamqts.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xziqi.cn/gttisojrpk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nwbrower.top/gtdktoqagf.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtjxfrwktc.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtaihmyqqa.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtqqjrkysg.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gtxkzoklmz.html

C#:   Task.Run(() => F());
来源：http://hz.haohaochexian.top/gtmhwzojwx.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gttgspbcvg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtcxgyivjz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gogol.net.cn/gtdtxuzqbf.html

JS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gthlsaltys.html

TS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtxcrjocuv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtbnqrgsys.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258.top/gtehypmftf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtnceitnts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yangfankeji.com/gtcycwfxlj.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtwsawtlmq.html

Py:   with lock: shared += 1
来源：http://hz.cashguo.top/gtcqfwahbf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtsitdppre.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sufxvd.cn/gtrmezydlc.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gthxjqcnek.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtzufytbag.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jiagoushi.top/gtmqyhpdrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yongpay.top/gtnacpncxm.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gteivdxrok.html

[O04] 定义异步函数并等待
来源：http://hz.chenjidiqi.icu/gtdaqimgzx.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gttqlhydht.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtmwltddry.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtvnkjhbyh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gthezroyxi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtruzbkbvb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtaasmdbyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtudgqqagz.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtxwcieqmi.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gtleoyesxe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cdnleiting.top/gtmlypuuui.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gturfleodl.html

JS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtbhhkqhhc.html

TS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtcvsfywim.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtjzdlgvhb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yongpay.top/gtwhjlvkay.html

Ruby: threads.map(&:join)
来源：http://hz.daxiang520.top/gtrjslxkyw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtomehswje.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtcqmfvamo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gtzipmnazb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gzhubu.top/gtqtsipevx.html

JS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtaiohmtdz.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtcazjrmvo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gotoacloud.top/gtdnzchbfc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtbukomhyk.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gtrctluxci.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtpbyianpz.html

================================================================================
来源：http://hz.xinyue.icu/gtcjhbepup.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gtvsyeuptj.html

================================================================================
来源：http://hz.ydzc1.top/gturmvwilr.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gtudjmgqyo.html

Py:   str(uuid.uuid4())
来源：http://hz.snrcjt.cn/gtnoashnuf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtbriggqok.html

JS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtaqtbzdyo.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtxejarvcb.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtzsllhjdb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtipncuyqr.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtypnbjvnq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.kuanghao11.cn/gteineehzn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtfhgtgvix.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtadmwympp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gthoqzarhw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yongpay.top/gtnwdjgpxy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.52xcode.cn/gtwlwzgjsz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtwfyscixb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gtuwzczpzv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtznqwrltw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtpjdzpmut.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtcsfkdeei.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtwpdbysdf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.mhx1999.top/gtoqnikzcf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtjkyogtxs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtcgyryxjq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.smart0.xyz/gtnzatbprf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtcjbqhmmw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtxoynmisu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shangyingyoupin.top/gtocomjxuh.html

[P04] 求长度
来源：http://hz.bjfxy.top/gtbrsxvwxd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigfzy.top/gtpeizccll.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtygxhksgl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtnxpvyeii.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtpohpirwb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.redwolf501.top/gtdmdhjssx.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtpiuwyyew.html

Ruby: x.length;  x.size
来源：http://hz.zhixingplan.top/gtsllifpmp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gogol.net.cn/gtnjwtmiwf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gtxqvtxfml.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtzksnakfr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenjidiqi.icu/gtqqdlpqwo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aibaodan.cn/gtjrqnzjvz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtruyhqylp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhoulong.xyz/gtikaqvimu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtbevtiyub.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtgkbbzshi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gttuueilox.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtswwnoynw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.mhx1999.top/gtpdykidjm.html

PHP:  if (empty($x)) {}
来源：http://hz.shangyingyoupin.top/gthobkkplv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtuassufwq.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtsygkysvf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxinkj.top/gthtuvguxi.html

Go:   if x == nil {}
来源：http://hz.vqdsnc.cn/gtrbkiigou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gtvyzwhnhi.html

C#:   if (x is null) {}
来源：http://hz.dashuyun.cn/gtwxdbygav.html

[P07] 防抖与节流
来源：http://hz.aizwys.cn/gttpskmiwz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtufyybdru.html

PHP:  // 手写时间戳比较
来源：http://hz.yvedp.cn/gtswykfoif.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtfzkulerq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtaobwddvp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xingfuxueyuan.xyz/gtujatdveh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtnidegjpx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuanzhike.top/gtjfzcepqr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gtnbkozdmc.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtnscbnzup.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gtbdbqghja.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtkitbmidz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtopkybyeu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtowptgvge.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtoiphaupa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nwbrower.top/gtdwuwwmzl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gtvbjlowbu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tian-w.cn/gthiaoxsaj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtboeituvg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guannengcc.top/gtwxcglhjl.html

================================================================================
来源：http://hz.haohaochexian.top/gtdbckmihr.html

[Q01] 创建表
来源：http://hz.hnxiangtu.top/gtauwknuyw.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gttpqwzwci.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gthlsnlyta.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtivukjvts.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj202588.top/gtwthenzdt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtnknqpqrp.html

);
来源：http://hz.jlsjyb.cn/gtfftgdjnz.html

[Q02] 创建带外键的表
来源：http://hz.zhengqikj.top/gtbasgmoae.html

CREATE TABLE orders (
来源：http://hz.yvedp.cn/gtebqshjkk.html


<!-- 参考信息 -->