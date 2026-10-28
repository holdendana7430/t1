代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.shangyingyoupin.top/gtkmonwnon.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtggfbnbmr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xinyue.icu/gtskcdvlvu.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gthqrxsufp.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtkiqivclz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhengqikj.top/gtwenptyor.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtxxmibcty.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtntxxofbm.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtypdztifd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtqykfhlom.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtcjlnhonr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cqqwz.cn/gtabjnahok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.iojbl.cn/gtsmoqchtp.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnysjfqpb.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtavdzilde.html

================================================================================
来源：http://hz.cashguo.top/gtwtmipjjf.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtbyqrhtgi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtkxvkhkok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtuvuyiyau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtlamehbwn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gteevrhdqh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuanzx.com/gtjorlcgzt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtkgfbtfgn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhixingplan.top/gtsrhmindb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtzfieuxns.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gttvhyjodq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtnexocaum.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtkvyxkfma.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtltkwqxkd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtvdkedzic.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtfvlwfxxy.html

Go:   slices.Sort(arr)
来源：http://hz.yuxming.cn/gttzknjqfw.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtyicderxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gttdraccia.html

[N03] 快速排序（分治示例）
来源：http://hz.cdnleiting.top/gtnjubwdqd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtopcqhhqn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yongpay.top/gtsssdassu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtehoolzmn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtxubwnbtq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daxiang520.top/gtlmucqncf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hywenlv.cn/gtkvxumuue.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtltiuynzc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtcbblhowu.html

[N04] 斐波那契数列
来源：http://hz.tian-w.cn/gtzkcyseso.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtasupfxun.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxinkj.top/gtexiqrpso.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtkoxmzdxh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtgndrpbuy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenjidiqi.icu/gtakyamjsc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.meibo888.top/gtftqbqwvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtbdlrigek.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtikipkbeh.html

[N05] 最大公约数
来源：http://hz.jinyuanbaomall.cn/gtlyskvuod.html

Py:   math.gcd(a, b)
来源：http://hz.bjfxy.top/gtbwmeuiww.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gtfgapcehz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtkvpzfszc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtjdesnxfe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hywenlv.cn/gtvnryurik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtgwkggdhd.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtlfwsxybf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtkimulnat.html

[N06] 判断回文字符串
来源：http://hz.jinyuanbaomall.cn/gtqrzmxifw.html

Py:   s == s[::-1]
来源：http://hz.aizwys.cn/gtwjqaqdnp.html

PHP:  $s === strrev($s);
来源：http://hz.jqgfzy.top/gtzytbusty.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtzxloysjp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gttqfiblux.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinyuanbaomall.cn/gthmlpmvfr.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtzethjozi.html

Ruby: s == s.reverse
来源：http://hz.feifeiyinyue.top/gtgvklmezf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtzvefnewv.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtepbjhfls.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hfpthk.cn/gttvrpuife.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtpxhgbwmj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinyuanbaomall.cn/gtcnwpuwdx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtodglaepb.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtzgramhhn.html

Go:   // 手写 map[int]int
来源：http://hz.hammf.cn/gtbadwudkt.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtiycplhde.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtyaekefwx.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtkofudyaj.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtosmayqwu.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtsjkbbqgc.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtaakvalcs.html

TS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtcdjkuebj.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtcslnoumv.html

Go:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtinxprxgg.html

Ruby: arr.permutation.to_a
来源：http://hz.yangfankeji.com/gtkjklsyjt.html

C#:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtzklblbrk.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtfewsnbwh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtugsbysyo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtoxhroecf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gtyyidkpbm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtbdwbujss.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtbdfjgmdl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gthdiceocw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtfqfnyrlt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtqzwbalbe.html

[N10] 链表节点定义
来源：http://hz.dashuyun.cn/gtnrtemwgd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gtwgxyvafn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtvwzjpauy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtfxwxspnp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtdhiacsji.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gtexgxopfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.andypj.xyz/gtghfzmnny.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtvekrclgg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtsyonsvmo.html

[N11] 二叉树中序遍历
来源：http://hz.xuetiantiany.cn/gtzhseejcz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pycfn.com/gtemagmhrz.html

PHP:  // 手写递归函数
来源：http://hz.fengsongda.top/gthgvoeyuf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gthkmfmrpx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtvvrldvpd.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gteluxefhv.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gttjrnwqjp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.andypj.xyz/gteufcwplu.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtldpfbftb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gttvbzqdwe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xziqi.cn/gtdjtcpphh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtevrphbmf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtballkhlg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gthjbvepan.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtbuvpjgpk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtmndyopum.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gthdbspsgk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtxjdvwtsr.html

================================================================================
来源：http://hz.shzxlz.cn/gtebyptnqq.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gthkbifjgd.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgaijaaei.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gttqlatlrs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gtocbvzsfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtomjhoffj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydzc1.top/gtibshtycf.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtaxlwxetn.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gthgomwetg.html

Go:   go f()
来源：http://hz.chenzaomai.com/gtgnxtswkb.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtuhmbexox.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtarrfwqst.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gtqxliiqvz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangkeji.top/gtrgxkwtlj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gtbsqflyle.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtonqpysmy.html

TS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtzwybfggg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gtljstmryi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.vqdsnc.cn/gtndfavuah.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jiagoushi.top/gtwuymmymn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtlvjpujch.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gtpvyamvhv.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gtvvqgpkwm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtofddhzin.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtdivpukgu.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtkajzngqj.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtqxsdubhg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydjk.org.cn/gtbddyglfs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtocpmwudb.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtxivclsqz.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtavlipmfr.html

Py:   async def f():⏎    await g()
来源：http://hz.sxryk.cn/gtaueyqaez.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtjyjabtwa.html

JS:   async function f() { await g(); }
来源：http://hz.zhoulong.xyz/gtzwgqyfry.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuxming.cn/gtljztfhzr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhengqikj.top/gtbsitjspi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ehwqpu.com/gtuvvvgdak.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gtutrmwpjb.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtzlsvyomo.html

[O05] 并发执行并等待全部完成
来源：http://hz.guannengcc.top/gttnogxvku.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gteaefivpm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtaddxxayz.html

JS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtqseyjmdq.html

TS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtfujafxtc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hywenlv.cn/gtxgpkfbby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtsjvguhtd.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtkfjibjxj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gttumbbiaw.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtcdxtgtfv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pycfn.com/gtrijowmqh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtaopjhdny.html

JS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtizojdlzn.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtemfchpol.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtvmfbqsgs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtaezkqxbx.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gtrdboltlv.html

C#:   Parallel.For
来源：http://hz.yj20258.top/gtbvoyapko.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwkojecqx.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtjbfgntfc.html

================================================================================
来源：http://hz.yj202588.top/gtzjrmetni.html

[P01] 生成 UUID
来源：http://hz.shzxlz.cn/gtsbdzpmea.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtgqqqwbmy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtzpptlfap.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtgimfqoqt.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtkzbbwahw.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtzwhlaedd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtgvfpuwum.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtiyofnjws.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jqgufenzy.top/gtzttxqzqi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtkfzuykvu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtkoxkrvqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgfzy.top/gtvglgbbif.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtnyjyijoz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtjmssoczp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gttuqjbkrl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtyacipsme.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtizfwmzcz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gtkyxraetp.html

[P03] 生成短随机字符串
来源：http://hz.ydzc1.top/gtaxmmbars.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fengsongda.top/gtgcovqutv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtnfuurjjy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtvxfrsunt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtptggfwyh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dianchejie.cn/gtcenqnpps.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cqqwz.cn/gtbfjeskst.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.316326.xyz/gtlxvnqsfl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtuxvkrvil.html

[P04] 求长度
来源：http://hz.aizwys.cn/gtlgocuzme.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.mhx1999.top/gtcuqyjaxm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtdknymren.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtbomabhxe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtqtefmmjr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtwjivhivu.html

Go:   len(arr);  len(m)
来源：http://hz.aizwys.cn/gtbpojtpat.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtewawcjgi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sweek.top/gtcimhaiwl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnxiangtu.top/gtkpeygxxm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtlkwfetwu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtntxkpust.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.vqdsnc.cn/gtcnxyherk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gteuvcluhw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gtgqugrpbu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtmlrxccna.html

Ruby: a == b
来源：http://hz.nanxuanxn.top/gtwnbgqese.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtstphmbkh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtzhqewbzw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuetiantiany.cn/gtlmeszgfs.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtukwbfzwy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtvirfgurg.html

TS:   if (x == null) {}
来源：http://hz.yuanzhike.top/gtokpianzg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtlsnlmtob.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtqhahsceo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zdqjudy.top/gtmaprbdpr.html

C#:   if (x is null) {}
来源：http://hz.shangyingyoupin.top/gtnqnoiram.html

[P07] 防抖与节流
来源：http://hz.jinqigufen.top/gtlfflzior.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnxiangtu.top/gtvycocvxn.html

PHP:  // 手写时间戳比较
来源：http://hz.guowangkeji.top/gtuynpzosi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtrijtmaqm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtwgrotket.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtyvgxpiyx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zdqjudy.top/gtjisplgfa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.feifeiyinyue.top/gtlmoinfrb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtxtwchwuk.html

[P08] 处理浮点精度问题
来源：http://hz.shangyingyoupin.top/gtxcrybokn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtrlpnuojn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shzxlz.cn/gtqiugmiys.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtahteovbw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtakjyszgq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jiagoushi.top/gtnthvqyjb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtspqpbmzg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.kuanghao11.cn/gtauoyxoho.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gaohongyu789.top/gtxnkzervz.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgqbniarg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gtcdujjjvz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtievgabdg.html

[Q01] 创建表
来源：http://hz.chenlongwang.top/gtlunlkocn.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtmaczhyyx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtarrggrry.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtsyvlrfkh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhiwuduotai.top/gtofiurclq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtpodveepr.html

);
来源：http://hz.zhoulong.xyz/gtovofqwlt.html

[Q02] 创建带外键的表
来源：http://hz.kuanghao11.cn/gtlyznhroo.html

CREATE TABLE orders (
来源：http://hz.gzhubu.top/gtazjqzccv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtlypwbmbf.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtobkcrdln.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtupvphahm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jiagoushi.top/gtehfnrwcx.html

);
来源：http://hz.gzhubu.top/gtnasysifv.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtuekujkph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtetkdtski.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtbnmkicxl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtijtcieva.html

[Q05] 重命名列
来源：http://hz.feifeiyinyue.top/gtvumpmomh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtwknvdtox.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtybrolbpa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cdnleiting.top/gtxjbrrleo.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtedubpiby.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gticsrjrsv.html

[Q08] 创建普通索引
来源：http://hz.jinqigufen.top/gtezckzaso.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gtenlnspza.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtgmdejlwt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtuwnzobot.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtgnpozqca.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ywan-chungtsiang.top/gtihoxtpgh.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gtvxhckayi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gteulhgpuz.html

[Q12] 插入后取自增 ID
来源：http://hz.snrcjt.cn/gtyodsvscm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtvlqmlhmf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gtkssuhwck.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtwfmukrgk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtnkjhohce.html

[Q14] 存在则更新（upsert）
来源：http://hz.ehwqpu.com/gtkdwqxxkw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtnrxmbngn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nwbrower.top/gtnkdzypsb.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gtsrvuyrhe.html


<!-- 参考信息 -->