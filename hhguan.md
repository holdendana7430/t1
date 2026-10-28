代发 wailian999

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtgajaurit.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gthnrvovbj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtfnfdivot.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gteofwttyt.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtqalrzjzc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtzbwcaosd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtjpddkuen.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gtcckvdzgc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtfjnnbqem.html

================================================================================
来源：http://hz.jiagoushi.top/gtlkwprwqy.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtedthsrzx.html

================================================================================
来源：http://hz.cheryme.top/gtegotxgcu.html

[N01] 二分查找（有序数组）
来源：http://hz.sysykeji.top/gtdvtqhefd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtownihcnj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtppysxfvk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtuyvkyngr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtokviwajo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.havefunace.top/gtzknmoihf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.9152youxi.cn/gtzvxpqaep.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gttwykebjw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtjwwoosxa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtbhgtrdlk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtzdejixen.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gttkrsngii.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtqddeyddw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtojvmcdvi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtzshnnwen.html

Go:   slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtybyszwur.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtkcakhctb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtzuujxufm.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gtvzuuauiw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtevnsoaio.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtivjrrjwh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtmhlnwltv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtiautllpr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtzykwbjqq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtiejomvwo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtxirdssxz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtdglcttvg.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtvwrxqfxb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtmlpszewq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtcrqtczhq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtswjwbyrl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtoxitqvgt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhijiandao.cn/gtifzfvdgo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fzhhl.top/gtlgthfpqd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtgsndsyju.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtckgpglql.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtetquuxmr.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gtguyqmbmx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hysaishi.cn/gthzanbnxk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtjdaapbyj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtvhgypxlu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtmtbdfbaa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtgperfwsq.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gttqiidhhp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ybcxt.top/gttkacmpfi.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtqzgpneij.html

Py:   s == s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gttbvrbpau.html

PHP:  $s === strrev($s);
来源：http://hz.nwbrower.top/gtdcwvfpij.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtcrcxdaij.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtaukmipkm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtslqocrsr.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtmubktjsa.html

Ruby: s == s.reverse
来源：http://hz.xinyue.icu/gttzjtrzdz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtukttlqmh.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtcxjeomqt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cashguo.top/gtvrperdzs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jyoumei.cn/gtkuqthoxu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sysykeji.top/gtopfpvzvv.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtoyjozkhk.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtzngssqez.html

Go:   // 手写 map[int]int
来源：http://hz.xziqi.cn/gtpxwefiox.html

Ruby: // 手写 Hash
来源：http://hz.hywenlv.cn/gtcrrljrtn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangdashe.top/gtnqbxnbxe.html

[N08] 生成全排列
来源：http://hz.jqgfzy.top/gtpxjbelzg.html

Py:   itertools.permutations(arr)
来源：http://hz.nwbrower.top/gtkgzjutmx.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtofmquiuq.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtyyyijxqx.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtbclprwnz.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtfniikqtb.html

Go:   // 手写回溯递归
来源：http://hz.hnqzz.top/gthtotjntw.html

Ruby: arr.permutation.to_a
来源：http://hz.guannengcc.top/gtvrmpvdxu.html

C#:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtawpbscsx.html

[N09] 栈与队列
来源：http://hz.daria6918.cn/gtkrkjrori.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangkeji.top/gtjcwquadt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zycfv.cn/gtpfdzrehq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ivvv.top/gtrhgtmaoa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.meibo888.top/gtlgmtsaye.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.0kj1m.cn/gtybehbknz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtjvggvwvh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gtvwjtaolr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jyoumei.cn/gtkbthwamv.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gthcbnrbwr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtiwioqeep.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aizwys.cn/gtmyvmrahq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gtgwwvdzza.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtmdrnaqul.html

Java: class Node { int v; Node next; }
来源：http://hz.zhaomingkeji.xyz/gtauedvuaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gtwiogurbl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aizwys.cn/gtbjnqlbff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dianchejie.cn/gtfyedowpe.html

[N11] 二叉树中序遍历
来源：http://hz.jiagoushi.top/gthkoaemuw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtaaytezyz.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtlpwtarvy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtepnriafu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtwlwdavct.html

Java: // 手写递归
来源：http://hz.yuxming.cn/gtuumrrhhy.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtidqrayma.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtwvhhvfga.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gteculwvuz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shangyingyoupin.top/gtcgcahjpc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gtzfwfyihp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gtfgoubryo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtiaohwaym.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtjpgpwgvz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtbqkujhyj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtrorwmjea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cashguo.top/gtjfaszmsb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtzryzicwd.html

================================================================================
来源：http://hz.cucudq.cn/gttxexwkbk.html

O. 并发与异步
来源：http://hz.ehwqpu.com/gtacwtohap.html

================================================================================
来源：http://hz.yanxiufei.cn/gtwunbrahp.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtscyfnbmy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtjxbfjtmq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gthufturrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yangfankeji.com/gtokzjsqzq.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtvcmfrcle.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtkvrprfwp.html

Go:   go f()
来源：http://hz.yongpay.top/gttoyyeqqn.html

Ruby: Thread.new { f }
来源：http://hz.zdqjudy.top/gtyqqswebp.html

C#:   Task.Run(() => F());
来源：http://hz.iojbl.cn/gtoxnockbv.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtlgktwbqs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhixingplan.top/gtwvrmgzlt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dianchejie.cn/gtclufrvgw.html

JS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtjgslhbxf.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtugupdxzy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtyorgxkfn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zycfv.cn/gtuyapsjlf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtnlpoppda.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtqugqkdve.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gtuxflcmda.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtxmznbqzs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtcrltisth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gtaqzckdgk.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gthvmsirxm.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gtluiekwvd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtwgzmmoky.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtrsxeetfo.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhengqikj.top/gtwzpxvzjj.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258888.top/gtygodfoof.html

Py:   async def f():⏎    await g()
来源：http://hz.redwolf501.top/gtixzzgaao.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zycfv.cn/gtvkkbajpe.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtdjopafmt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtvtribmjs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.c1oappe.top/gtaderfnms.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dashuyun.cn/gtwafjyhfr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhaomingkeji.xyz/gtgsfdkvqa.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtbmejvzws.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtlayvlqey.html

Py:   asyncio.gather(*tasks)
来源：http://hz.52xcode.cn/gtojoynfbx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtgznjpqiq.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtosnuesek.html

TS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtiotjtwpf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtnpcspkhx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xingfuxueyuan.xyz/gttysvwsla.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtwjkwiaru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jianghu66.top/gtkqsdyscr.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gthsdcwwlf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ppjwa.cn/gtihzyyvxr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtiqqrxknh.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gthdiuqxhk.html

TS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtmntcijnp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtiwnycgmk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yueranfly.top/gthggqslpr.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtdynayxxr.html

C#:   Parallel.For
来源：http://hz.pengpengdd.cyou/gtpyayjxvy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttnsseoya.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtzjhwsvxo.html

================================================================================
来源：http://hz.nwbrower.top/gtnkqonzld.html

[P01] 生成 UUID
来源：http://hz.yj202588.top/gtbqeselyi.html

Py:   str(uuid.uuid4())
来源：http://hz.aizwys.cn/gtpkhhkeez.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtzezoqdnh.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtxaerlwdh.html

TS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtwnrlgbqh.html

Java: UUID.randomUUID().toString()
来源：http://hz.shuidangran.top/gthpkygvke.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtmglemslv.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtttuedlgp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gtnddbrdsg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yonumen.top/gtfyvfudxm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ywan-chungtsiang.top/gtmrzkzliv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinghuilouyu.cn/gtcvgybnwi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gticppmbqi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtqldnxohw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtznkazsmy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gthfkrcikb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gtsetixohb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtnjoikqcp.html

[P03] 生成短随机字符串
来源：http://hz.jiagoushi.top/gtwdryezvt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258.top/gtqzpmjfnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gtlxrsghzg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtxowrakbs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtbsygccoi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtstrdfott.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.meibo888.top/gttmzulzcm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtruxphpex.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtqfjshpyj.html

[P04] 求长度
来源：http://hz.hnxiangtu.top/gteenfyioi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sweek.top/gtkuaqybfh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtogafblbx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtttdoutst.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtfsryiaru.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hfpthk.cn/gtspwycfjm.html

Go:   len(arr);  len(m)
来源：http://hz.tianlin.xyz/gtprhuabni.html

Ruby: x.length;  x.size
来源：http://hz.jlsjyb.cn/gtcucivfan.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtxtgcxgnh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xylfe.cn/gtgfjpelcx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sxryk.cn/gtzseakafn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cashguo.top/gtkuezjqmy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydjk.org.cn/gtwurbhejm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtxpgepsvp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dianchejie.cn/gtjxurpodu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtznpegfjd.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtuhgeievm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yueranfly.top/gtouzudnoj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtmynlquut.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtynyokxeu.html

PHP:  if (empty($x)) {}
来源：http://hz.yuxming.cn/gtcmzaqnrv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fengsongda.top/gtqiqjmvdj.html

TS:   if (x == null) {}
来源：http://hz.chenjidiqi.icu/gtufptdfoj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtoceofuww.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gthrucevvi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ppjwa.cn/gtzldjzdvv.html

C#:   if (x is null) {}
来源：http://hz.ppjwa.cn/gtlwpyyewa.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtrgtgtauz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtmmsbyhnj.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtyqelbxtj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtydzietls.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtnmwhkxfy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtmhijlcvp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtzwhdnxqu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuxming.cn/gtqvrzcrca.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtildlzsol.html

[P08] 处理浮点精度问题
来源：http://hz.daria6918.cn/gtfzozswjx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtncbtopzc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shzxlz.cn/gtwexxwhgl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.52xcode.cn/gtjxxgiqtw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gogol.net.cn/gtbfmuwrgv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtppbiwoqg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hongshengwenyu.top/gtveushqfe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tian-w.cn/gtwczuyvdn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtdzaljbrt.html

================================================================================
来源：http://hz.cucudq.cn/gttxilfhqi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cqqwz.cn/gtucrugzcj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcgqapskh.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtdyjmndlw.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtruftveyg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtspykwpzs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gthznnpqse.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gttfvkcscl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nwbrower.top/gtvckxulte.html

);
来源：http://hz.havefunace.top/gtuauouhle.html

[Q02] 创建带外键的表
来源：http://hz.fengsongda.top/gthkurxogv.html

CREATE TABLE orders (
来源：http://hz.hywenlv.cn/gtzgmdjsug.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.quarkkingdee.top/gtisicqonx.html

user_id INT NOT NULL,
来源：http://hz.chenjidiqi.icu/gtpguvbnld.html

amount DECIMAL(10, 2),
来源：http://hz.iojbl.cn/gtwasmrtew.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtuvfvojup.html

);
来源：http://hz.sweek.top/gthdynxacn.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gttjksfwcv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtbkcgiypx.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gthtmrilbx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtcrhefpun.html

[Q05] 重命名列
来源：http://hz.yj202588.top/gtasllbbji.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.snrcjt.cn/gtupmtfffn.html

[Q06] 删除列
来源：http://hz.cucudq.cn/gtpnwoebxo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jianghu66.top/gtsntgyyzs.html

[Q07] 删除表
来源：http://hz.zhiwuduotai.top/gtcullisqi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtnvwifstt.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtyefoxaps.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gttudlqqpo.html

[Q09] 创建唯一索引
来源：http://hz.xylfe.cn/gtulabxzqd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtxdredmte.html

[Q10] 插入单行
来源：http://hz.zhaomingkeji.xyz/gtrcgbdtcc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shuidangran.top/gttyhdwqqp.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtvetadixn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtoslazsfn.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gtxcrlykel.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtsmkuqigx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fengsongda.top/gtbwmleksc.html

[Q13] 忽略重复插入
来源：http://hz.yonumen.top/gtqafibuun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtoayynath.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtkqwceowm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ehwqpu.com/gtsqakwzcp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtseuxxzuu.html

[Q15] 查询全部
来源：http://hz.birdmap.top/gtbopvfycr.html

SELECT * FROM users;
来源：http://hz.feifeiyinyue.top/gtembzbsvp.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtgpdlvrqg.html

SELECT id, name FROM users;
来源：http://hz.quarkkingdee.top/gtnkttyxsz.html

[Q17] 条件查询
来源：http://hz.tianlin.xyz/gtjcoibmpd.html


<!-- 参考信息 -->