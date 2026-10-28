代发 wailian999

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtmguzwwmo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guowangkeji.top/gtiwaeizkz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtcskcdswt.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gttiezdhdr.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtmnsulngy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hfpthk.cn/gtxffpcmad.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtuqcvxyny.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yueranfly.top/gtbpjgaupz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtrdvyykad.html

================================================================================
来源：http://hz.haohaochexian.top/gtlkbuuyvu.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gtjfnqlflu.html

================================================================================
来源：http://hz.gogol.net.cn/gtdfemxabs.html

[N01] 二分查找（有序数组）
来源：http://hz.tian-w.cn/gtklmsjcwh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtoysmvwfv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtigzludba.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtlqxfcqew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtojmgqggx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtzbksrsqg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gaohongyu789.top/gthlevhxph.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj202588.top/gtkyduresy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtjauhjeky.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gttwxvmcls.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtnppafnsi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtqnnxtfbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gteczyumvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtsozocybo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xingfuxueyuan.xyz/gtgxrfaedt.html

Go:   slices.Sort(arr)
来源：http://hz.yuanzhike.top/gteimosdkx.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtgnxfddsi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guowangkeji.top/gtucjuhsso.html

[N03] 快速排序（分治示例）
来源：http://hz.pengpengdd.cyou/gtvwevpogx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhijiandao.cn/gtoheqyocj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gogol.net.cn/gtgcostuuj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gthxkloxjr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtazowtcih.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gthkyfmrni.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gtdtmohvny.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.haohaochexian.top/gtpjiinxlp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtmaxrlqft.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gtxjoziqqh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtyumstyzo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgufenzy.top/gtdnmvcesf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtvtqddwmo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtajwmznmc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtrjshytbf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gtxxtyrnsc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtnvghzsvv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtluqubhub.html

[N05] 最大公约数
来源：http://hz.c1oappe.top/gtjkvyoiyp.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtgsemnvpm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.haohaochexian.top/gtfrovebvd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtwwhujplt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtifudfwna.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gtftzelhqz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.meibo888.top/gtvqvxbhsr.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtnnpnrlrq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtepwidhmx.html

[N06] 判断回文字符串
来源：http://hz.guannengcc.top/gteocezret.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtcepainvp.html

PHP:  $s === strrev($s);
来源：http://hz.zdqjudy.top/gtgmdzmfjm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtljmtcfld.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtmojtbcwu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtdivsugow.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtthusipds.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtsgmgrqri.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtcgypryww.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtgeoxsuet.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.bjfxy.top/gtspdeyzdu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daxiang520.top/gtgkwgdgni.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtjcpkpero.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtcigcykjj.html

Java: // 手写 HashMap
来源：http://hz.havefunace.top/gtdgpqshxk.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtdwlbxojn.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gtqwlgzljx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gtztehdmru.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gttvfllewp.html

Py:   itertools.permutations(arr)
来源：http://hz.mhx1999.top/gtqnjjkmiq.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gthhubmnxt.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtyalpfdsy.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtjobnhfsy.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtkfdlrffu.html

Go:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtxlbjniqq.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtqglzfxze.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtqjzoabjs.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gtvbyzebbk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jianghu66.top/gtobixvjhl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guannengcc.top/gtrcbqdptp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtmcqftgzf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtuoywbyef.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtjsxhfgbz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtcgymecdp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtrqvzsspk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gtomllktwk.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtmmuzbdfj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gtwsgwqrjs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtnwfaagqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtsqguwwir.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.316326.xyz/gtaudpnagl.html

Java: class Node { int v; Node next; }
来源：http://hz.zhiwuduotai.top/gteuvkvzwv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuxming.cn/gtajwgptys.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtzeaowcgn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgufenzy.top/gtexqtpmgb.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtmgqbugrl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daxiang520.top/gtivwaddve.html

PHP:  // 手写递归函数
来源：http://hz.jinyuanbaomall.cn/gtjvvuffpa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtkbguyxev.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtidunruey.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtxfegmcqq.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtouikymjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtpeldybcp.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtgsporzni.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhengqikj.top/gtaaaogjgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangshuangyany.cn/gtdnrlypwk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtqnvkwtho.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtbjsbsvpp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtdtghebfd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gthaznbjcz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtsquimhpc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinyuanbaomall.cn/gtaaequlmy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtwvxywiox.html

================================================================================
来源：http://hz.tanke756.top/gtmtmtjsrl.html

O. 并发与异步
来源：http://hz.redwolf501.top/gtowfogotv.html

================================================================================
来源：http://hz.gzhubu.top/gtbtftigdh.html

[O01] 启动一个线程
来源：http://hz.zycfv.cn/gttjvwltdv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zdqjudy.top/gtysomuetq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hammf.cn/gtovnjtent.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ywan-chungtsiang.top/gtffwupctb.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtatjfqjth.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtzutspzzm.html

Go:   go f()
来源：http://hz.fzhhl.top/gtwpzqulcz.html

Ruby: Thread.new { f }
来源：http://hz.yuanzhike.top/gtycamfkmi.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtnxdsdjyt.html

[O02] 使用线程池
来源：http://hz.cheryme.top/gtnievoaba.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gthnqaxxls.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtabekbmhg.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtxlcgzfoc.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtdnlixthn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtpfkhcezy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtfvyikrwq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cqqwz.cn/gtbocpxyis.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtvdenlzms.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtoqvcgbud.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtxtmlunse.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenlongwang.top/gtpcndfzwn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtbnsyitdt.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtnhtgetee.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gtdlqtqdve.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtxggrpbqg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.smart0.xyz/gtozcozygc.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydjk.org.cn/gtyadwgafy.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gtqkryiyqn.html

Py:   async def f():⏎    await g()
来源：http://hz.shangyingyoupin.top/gtttwggkss.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtseudvlsj.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtbgcwupyj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gtnxywqmjk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sysykeji.top/gtnwvwikxx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cashguo.top/gtdkbkpylu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangkeji.top/gtveczagqk.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtzyaqumrc.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtdhjtizzd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtppkxxtby.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gthqsjjzec.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtfmagzkrg.html

TS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtyjioolhi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gotoacloud.top/gtkcsbxxwq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fzhhl.top/gtpkhgecqs.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtcaxplwxe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtpczbqnln.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtzuodpnbj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gtnuuoytej.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hammf.cn/gtctwrvsbj.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtnjhkcsdd.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtabwgzenl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigufen.top/gtymugutkt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.snrcjt.cn/gtaxpmzuqg.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gtcrrqjdub.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtbspolcel.html

================================================================================
来源：http://hz.jinqigfzy.top/gtynbziswz.html

P. 常用工具函数
来源：http://hz.hongshengwenyu.top/gtsgmknobk.html

================================================================================
来源：http://hz.ehwqpu.com/gtzmgfkkeg.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtwztsahoy.html

Py:   str(uuid.uuid4())
来源：http://hz.feifeiyinyue.top/gtdxlvwauw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xinyue.icu/gturcwonta.html

JS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtumqwhiap.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtbilhpymk.html

Java: UUID.randomUUID().toString()
来源：http://hz.tianlin.xyz/gtianetrkx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtvffaifif.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gturikjxvb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtpujupgjj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fengsongda.top/gttizfemxf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhixingplan.top/gtfeoevvpe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtgxcfldpc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guowangkeji.top/gtuewqonvu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gotoacloud.top/gtrdwglnko.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtjueguvkm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.quarkkingdee.top/gtyxhxahwn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.haohaochexian.top/gtsrcflfxt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ivvv.top/gtjdlvknzo.html

[P03] 生成短随机字符串
来源：http://hz.snrcjt.cn/gterjphgxp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tian-w.cn/gtmvzilbmv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gthxyeyamv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtxryylrgs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtzvtjshgj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtzyuqohvg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gtovbiycwv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hfpthk.cn/gtmrkkfkzn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtnnllzhrl.html

[P04] 求长度
来源：http://hz.yj20258.top/gtapmsqzbo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtireerdjv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtzmszuupt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtgfzhlevl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtakobhqpd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigfzy.top/gtdigzdsfb.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtqitnmumt.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtcwballik.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhoulong.xyz/gtmuwquzfl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zdqjudy.top/gtmiodfgtl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtlswhsltf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtdpqbdswv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gttvsprzxv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnxiangtu.top/gtnjrxmssc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ywan-chungtsiang.top/gtaiizbqzq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gaohongyu789.top/gtpshjoqpe.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtawzfbbvw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtupznbzok.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtowqhsdol.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtipbzwtbm.html

PHP:  if (empty($x)) {}
来源：http://hz.0kj1m.cn/gtrnhpctna.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gtsyppbghh.html

TS:   if (x == null) {}
来源：http://hz.316326.xyz/gtslavjnwv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtmqdfnial.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtaaymxdjj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tianlin.xyz/gtbqjpmvhv.html

C#:   if (x is null) {}
来源：http://hz.ehwqpu.com/gtukshcqbw.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtwihmkgdx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fzhhl.top/gtubxnertt.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtcdxniljl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtbzknbaxz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtuycyguhp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtfabsevun.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtjxtmldez.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gtvmaydnhg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cqqwz.cn/gtlbyrvolz.html

[P08] 处理浮点精度问题
来源：http://hz.shuidangran.top/gtswnghrhe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gthccqbsmv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtylzsqggu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtfjmaccdr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhoulong.xyz/gtsyaqkrxr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtnkyqytlz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.feifeiyinyue.top/gtdrnmupsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj202588.top/gtirlmnujn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgfzy.top/gtbgwqcsqa.html

================================================================================
来源：http://hz.yuanzhike.top/gtegmoeepw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gtsmcbntcm.html

================================================================================
来源：http://hz.kuanghao11.cn/gtjpcnfuvt.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtlvllacgf.html

CREATE TABLE users (
来源：http://hz.jlsjyb.cn/gtlyrpgnzt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtjxtybuta.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yangfankeji.com/gtcucstsiq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj202588.top/gtpacgekhf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gteekeefjk.html

);
来源：http://hz.cucudq.cn/gtomvahsve.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangtech.top/gtichxdfne.html

CREATE TABLE orders (
来源：http://hz.zhiwuduotai.top/gtwssytdwr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtnnggnauy.html

user_id INT NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtuojllkbc.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtycumpjgh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtkyegmmxk.html

);
来源：http://hz.guowangkeji.top/gtykkhbazq.html

[Q03] 增加列
来源：http://hz.nwbrower.top/gteboiorah.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtqgntovfb.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtnwndcjmi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ybcxt.top/gtmcdsoqdh.html

[Q05] 重命名列
来源：http://hz.tanke756.top/gtlajmmpoh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gogol.net.cn/gtdsumgmlz.html

[Q06] 删除列
来源：http://hz.redwolf501.top/gtnlgqghyv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gtjeeybvrx.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtlbgbcpkh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jlsjyb.cn/gtzirliatr.html

[Q08] 创建普通索引
来源：http://hz.jqgufenzy.top/gtbnutkkmq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuxming.cn/gtslzxpnzk.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangtech.top/gtwsqwlvnw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtigupubyz.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtbilmxdhy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtdqtlgauh.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gtljbltnew.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtsgdpsnvu.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtveovfkte.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yangfankeji.com/gtizsjeczm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.iojbl.cn/gtvndylsmj.html

[Q13] 忽略重复插入
来源：http://hz.hywenlv.cn/gtwteqxfeu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nwbrower.top/gtpkbzwbgq.html

[Q14] 存在则更新（upsert）
来源：http://hz.redwolf501.top/gtlzuaghho.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtzuuiciiu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gtuugziyto.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtcrvcewwy.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtfypybjzl.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtalzfgvoi.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtfyupxnye.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtupunajkd.html


<!-- 参考信息 -->