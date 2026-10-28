代发 wailian999

[M08] 获取系统与运行时信息
来源：http://hz.jinqigufen.top/gtpmmecigz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gtfgsyuret.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtkcsnxzfc.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtnmlzhvsg.html

TS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtmyrghtis.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtbxadoyxp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtxgwsbbvr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtnofkrycj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtfcemtgba.html

================================================================================
来源：http://hz.cdnleiting.top/gtaclenjbj.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtrmrkexlr.html

================================================================================
来源：http://hz.xinyue.icu/gtrfjbbnbl.html

[N01] 二分查找（有序数组）
来源：http://hz.52xcode.cn/gthjagqofb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtzmnckjie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtoncwjhvg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtqcwsesdb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtyacxavti.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtncjprvir.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtupjpowop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtghnpzkuc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtjevucahk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yangfankeji.com/gtyqzrdmoh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtueghypnl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtosigeevt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtxevszgvi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtwgnfommd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtstnsqxmq.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtlskytyfu.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gthrcvvygk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtfynkktsn.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtsbsnaaax.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtcqtxxjzq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxinkj.top/gtwvuatlwk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtayjlpnga.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtjxokilzs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtqqzrthuk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtcryeawka.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgfzy.top/gtjaklsofd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.andypj.xyz/gtynzyumvs.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtbodblgxw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtzgjbujry.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtavemzmfk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtcaciskwg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtvhvbvrok.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtnzggpkkk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cashguo.top/gtooxsupqk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtdkzgovkx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtszrbcuom.html

[N05] 最大公约数
来源：http://hz.ydzc1.top/gtusxzgpyu.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtxwezftdb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtvgjiqvle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtgozzgqhh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtdsecmihv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gttueaxwjn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigufen.top/gtdxtjvmgn.html

Ruby: a.gcd(b)
来源：http://hz.mhx1999.top/gtugmvjvxh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtdylxvwko.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtcatzvewz.html

Py:   s == s[::-1]
来源：http://hz.birdmap.top/gtfyhottyj.html

PHP:  $s === strrev($s);
来源：http://hz.haohaochexian.top/gtikjgxtsb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtbjjbnhvv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtkkvofeew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.birdmap.top/gtkdejjbim.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gtmdedgvwl.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gtvfnqrxyb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtcehbhbjr.html

[N07] 两数之和（返回下标）
来源：http://hz.nwbrower.top/gtjylmpaak.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pycfn.com/gtpiruopcz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tanke756.top/gtgppgyjuu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtcjcxpbyv.html

TS:   // 手写 Map<string, number>
来源：http://hz.ppjwa.cn/gtypxiisda.html

Java: // 手写 HashMap
来源：http://hz.xuetiantiany.cn/gtoiyabcws.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtkmplgnjg.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtwkbcregt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtpfegduct.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtqeopbmqe.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gtqtdfsvyx.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtwudicldq.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtopemwxkw.html

TS:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtgubdbdsm.html

Java: // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtpyleltud.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtqyqoqetc.html

Ruby: arr.permutation.to_a
来源：http://hz.hywenlv.cn/gtxnbsdzrf.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtrmnkiaof.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtyendonnz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtsrupohmw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guannengcc.top/gtzkoxkbfo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gtehhinuej.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtvxosnedn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xinyue.icu/gtghumcaub.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtwunstmvn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtbxdxqobx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xinyue.icu/gtfiraecnt.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtqzbnkufn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtopfhyhwf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhaomingkeji.xyz/gtkrbapwhv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pycfn.com/gthyipebwm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtgvjnefra.html

Java: class Node { int v; Node next; }
来源：http://hz.xuanzx.com/gtwjesghjk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gtmilbyqpc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtzagpcobb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhaomingkeji.xyz/gtikuxarpp.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtzbhzfuaf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtkfmcqpqx.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gtmtlhjmky.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtdfhnzzuj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtpjqrrfsz.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gtcyqsjprp.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtabextiup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtjmrwezbo.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtyfonuvmv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtkrmvwmou.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ywan-chungtsiang.top/gtgposkqbg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtyukvjafn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtqfccxsee.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtzpdkoptw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtcvsjtqio.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yangfankeji.com/gtgzqovdke.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangtech.top/gtneqjlmuc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtizxwpvnh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcghzvgfk.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtenujxxfv.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqeiixmxh.html

[O01] 启动一个线程
来源：http://hz.xinyue.icu/gtbusqzdrp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtvzicsvfx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zycfv.cn/gtuufnrfce.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtafkmklfp.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtczycotly.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtfkscddns.html

Go:   go f()
来源：http://hz.nwbrower.top/gtrpxgivim.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gtnnsqmxte.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtsthiveth.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gteuewzcih.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtnosjyonr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yanxiufei.cn/gtfkbfvrlw.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtwjcfcabp.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtagtjazjp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangdashe.top/gtsqimgkel.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtdvcikatf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gteykdthfn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.redwolf501.top/gtqspeiujo.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gtgajgkfqt.html

Py:   with lock: shared += 1
来源：http://hz.hysaishi.cn/gtgnirkzia.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangdashe.top/gtrhpwxtxg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtnwfzbayj.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtwqkuwlgg.html

Java: synchronized (this) { shared++; }
来源：http://hz.hfpthk.cn/gtwxugaoaz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtffrfdick.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnqzz.top/gtjtkgalsw.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtqbhudlhj.html

[O04] 定义异步函数并等待
来源：http://hz.zhoulong.xyz/gtfuhrprbl.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtvqwndxdc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.andypj.xyz/gtlmchjdvn.html

JS:   async function f() { await g(); }
来源：http://hz.nanxinkj.top/gtqpfwnwop.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtbhrzhfas.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhongyouzk.top/gtzatccgoj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gthwyartai.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gtyqxbnyjh.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxinkj.top/gtdbgftpel.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtltcpjwqk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yvedp.cn/gtmtqeqiit.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtqqgodybv.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtvsbucqwq.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtwkhkxcfp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtwklkrdbd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sufxvd.cn/gtvvbvupry.html

Ruby: threads.map(&:join)
来源：http://hz.0kj1m.cn/gtpikptgfp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangdashe.top/gtpqusuaif.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtpybhiawu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtofsidiwl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gtxfeevdrp.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gttsuipeum.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtftatlvmb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daria6918.cn/gtbbmfypci.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtmovnortf.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtryyeqdhq.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtipokiosz.html

================================================================================
来源：http://hz.hammf.cn/gtetrskydr.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtlmovapck.html

================================================================================
来源：http://hz.yanxiufei.cn/gthfbhbogh.html

[P01] 生成 UUID
来源：http://hz.zhoulong.xyz/gtgxjtseoi.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtphlhvwrc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnqzz.top/gtuzpmrwut.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtuscacsmf.html

TS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtksbsaclg.html

Java: UUID.randomUUID().toString()
来源：http://hz.pycfn.com/gtluuwcxgm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtazyflgjl.html

Ruby: SecureRandom.uuid
来源：http://hz.iojbl.cn/gtlciczawk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhengqikj.top/gtbiqsfcmd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258888.top/gtfeuhiyuv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtmumhegux.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gthsupvpzy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dianchejie.cn/gthwoxddti.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cqqwz.cn/gtnayvrskp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhongyouzk.top/gtvdbywfnh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj202588.top/gtuwbrdwwm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtumtjovkf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtjlstuuol.html

[P03] 生成短随机字符串
来源：http://hz.daxiang520.top/gtmcbwvyaq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xinyue.icu/gtzcetezzq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gzhubu.top/gtzfdssnic.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtyzqwisil.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtspmhfiod.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tianlin.xyz/gtzacvzocx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtpacvccof.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gtxybtaigr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtewgaxvvp.html

[P04] 求长度
来源：http://hz.gotoacloud.top/gtjzlqwggu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cheryme.top/gtnlfsqtan.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtvsrtwxdm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtqkkszclc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtysvwasoo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtqrlckrhv.html

Go:   len(arr);  len(m)
来源：http://hz.gogol.net.cn/gtkgwfjazk.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtmbapmuvy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtahyqhquj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hongshengwenyu.top/gtbnfhmczl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gtrmpttxzd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxinkj.top/gtjaxxfihg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cqqwz.cn/gtzizpoyen.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtpxpwbhbk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.vqdsnc.cn/gtcdhokhjg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgufenzy.top/gtkmlnndpb.html

Ruby: a == b
来源：http://hz.quarkkingdee.top/gthtugcbgd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shangyingyoupin.top/gtbltwlsli.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtwzaqqobb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.birdmap.top/gtcmmwzmph.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gtorqebcah.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtxmmwxcke.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gtnrtzpzbu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtnqblemrq.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gthkhamsvr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtkgdpmdtu.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtuszmvwgr.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtzjwlokue.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gthhathpuf.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gtcceixayl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtjfebljpw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtrwybkdsn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hysaishi.cn/gtyehffzgx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtmbtndmfa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtbpukgugj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtsxsmneip.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtzmjuzled.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtcbriunvz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuanzx.com/gtzoevuisw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gtpwuyectb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gtohkhneoc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtjgvuzstk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxinkj.top/gthuvlbgyg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtkedqrlts.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtipfrwtjk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtspsacbze.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yonumen.top/gthnndolzl.html

================================================================================
来源：http://hz.gotoacloud.top/gttbdbpqds.html

[Q01] 创建表
来源：http://hz.hnxiangtu.top/gtkibtnqgr.html

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtvtkaapro.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtjuxmahjl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cheryme.top/gtyajpyluy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gzhubu.top/gtqzlshjze.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zycfv.cn/gtxdeyrnal.html

);
来源：http://hz.yvedp.cn/gtvffbbqsd.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtmaoxwjuz.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtqidknvbj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gtnfmcwkcu.html

user_id INT NOT NULL,
来源：http://hz.jinqigfzy.top/gtevruyils.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtgkcoqgrp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtbpwdifud.html

);
来源：http://hz.sysykeji.top/gtvaovvbkz.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtnckgbmab.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtbhnniyzt.html

[Q04] 修改列类型
来源：http://hz.ehwqpu.com/gtxbjfsckv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gthdsayaek.html

[Q05] 重命名列
来源：http://hz.xinyue.icu/gtdyvgyfib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangkeji.top/gtarobswla.html

[Q06] 删除列
来源：http://hz.yueranfly.top/gtiqpbmxpv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yongpay.top/gtwdqvshdt.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gtvtncfevx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtlyxgtorp.html

[Q08] 创建普通索引
来源：http://hz.zhengqikj.top/gtdjlcjdkd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtqigewmmr.html

[Q09] 创建唯一索引
来源：http://hz.sufxvd.cn/gtuycyuuqa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtcbcluspu.html

[Q10] 插入单行
来源：http://hz.zhijiandao.cn/gtawbsmpiu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yvedp.cn/gtzarazeft.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gtieqmfiyw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhongyouzk.top/gtohnilpxu.html

[Q12] 插入后取自增 ID
来源：http://hz.hywenlv.cn/gtroweuuxs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtyjgncbgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtfqlqyolv.html

[Q13] 忽略重复插入
来源：http://hz.havefunace.top/gtyhetovvd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.birdmap.top/gtgbnbwyeq.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtmlwmymcb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.andypj.xyz/gtcsvtmxvq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtxlglojjj.html

[Q15] 查询全部
来源：http://hz.redwolf501.top/gtltrqgvrl.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtpdooehlm.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtnnrphtsx.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtsxttgpmm.html

[Q17] 条件查询
来源：http://hz.hammf.cn/gtvzxijfaf.html


<!-- 参考信息 -->