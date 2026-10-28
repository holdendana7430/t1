代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtzmzepdzt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtweigvjtr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtuycoovhm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtgybvgddq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtciaorptx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtvfldozme.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtrpnqawqs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtnsntmqfw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtivabhbvj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zdqjudy.top/gtnesjxmgj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtuphwcpcj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtmgffxocm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtfezefmmr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gthpolgiax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cucudq.cn/gtcdyjmhpg.html

Go:   slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtkcsihkew.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtqmkcgllg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gtubdqimew.html

[N03] 快速排序（分治示例）
来源：http://hz.hnqzz.top/gtkklanrzi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhiwuduotai.top/gtzhkohgmd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtzfmbeqkp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtufkdlkno.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtjrkgxnvh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtshdowcbv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtksnmqjdp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fengsongda.top/gtjijragzz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pycfn.com/gtbnaqcwhp.html

[N04] 斐波那契数列
来源：http://hz.xuetiantiany.cn/gtykmcifgx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtfnyaspod.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtcbqfxgkw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtoehxuggk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtaiaprqvx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtgfjteyja.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtzwcyenjd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtkuqgxsyz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtkfvnjsvy.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtglhgzrfy.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtkzmibaof.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gtiejnwyjt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtbqrttcva.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtuaaxovxx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtqegenrhb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtfhihszxq.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtpooinyha.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgufenzy.top/gtwsnavbqf.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtmrqlkzyk.html

Py:   s == s[::-1]
来源：http://hz.yonumen.top/gtmfxwaope.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtvrgckevt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtkblxzolz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtfcaitlas.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ppjwa.cn/gtqayrblvu.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtasoravnn.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gteanckqrs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtqeazsisa.html

[N07] 两数之和（返回下标）
来源：http://hz.xziqi.cn/gtijjuzijz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtbazsyjrh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zycfv.cn/gtzmgezhlg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zdqjudy.top/gtyajmvlmc.html

TS:   // 手写 Map<string, number>
来源：http://hz.havefunace.top/gtqimcjvyr.html

Java: // 手写 HashMap
来源：http://hz.tanke756.top/gtskrsqglp.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtzseokikq.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gtcrjrsmsq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.0kj1m.cn/gtjwxvaysd.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtrntudfti.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtntgtfhvk.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtxxzytupe.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gttdlqoigv.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtnlfnxkae.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtkhlpukae.html

Go:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtwjhgcrje.html

Ruby: arr.permutation.to_a
来源：http://hz.jinghuilouyu.cn/gtckgckjjw.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtfamevmyw.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtnvvnrqzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.smart0.xyz/gtmdvhcmgk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtwudorpaw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtctzbrfrh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtwkmyayel.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtbkxfmovt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhixingplan.top/gtrnvnpsnl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtceyfzqli.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtdyrxjmlh.html

[N10] 链表节点定义
来源：http://hz.haohaochexian.top/gtdlbqkndh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtmlibnwmn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gtkjmpqjss.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtxoayyfie.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtebnbknhj.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtvotjurar.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jianghu66.top/gtbmyaprkp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtfudfdllw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgfzy.top/gthnkpsqed.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtbhpdzolq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jyoumei.cn/gthkrdrios.html

PHP:  // 手写递归函数
来源：http://hz.zhixingplan.top/gtyetyfxtj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtmaxrzsjs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtyaokckka.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtzidfolhd.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtnsaufznx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtlikjagyn.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtmsdpcdki.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.andypj.xyz/gtsqzeumlz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtyvkdhfov.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gtjfvhiklj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtguvrhkva.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtvwrcwram.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtzumeutnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtrvpcklpt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtzcrdmkpp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtvxlhqmzb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgawscddw.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtjlwqxowr.html

================================================================================
来源：http://hz.mhx1999.top/gtpuligbvv.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtdcgyfeuz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aibaodan.cn/gttcpvihys.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gtscsxnkqr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtvjfmwnie.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtouziwops.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gthtiqyakj.html

Go:   go f()
来源：http://hz.fengsongda.top/gtaaeneyik.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtvwqcxhnj.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gtziqdlovg.html

[O02] 使用线程池
来源：http://hz.iojbl.cn/gtpehjznqs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258.top/gtsflkytem.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cdnleiting.top/gtxncsjufu.html

JS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtugtdgund.html

TS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtnaplhzbp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtlqfxyddx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gtedbsnaiu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtzwbdgiwm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhixingplan.top/gtjylophjb.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtqjnuarnq.html

Py:   with lock: shared += 1
来源：http://hz.gogol.net.cn/gthnbnskxh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tanke756.top/gtoggeigyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtimxhimlm.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtoidictzq.html

Java: synchronized (this) { shared++; }
来源：http://hz.dashuyun.cn/gtjisgxvif.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gtiguopbop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtrfktbnhq.html

C#:   lock (gate) { shared++; }
来源：http://hz.kuanghao11.cn/gtrobbhjet.html

[O04] 定义异步函数并等待
来源：http://hz.hywenlv.cn/gtufdvxmky.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtckxrckjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuanzx.com/gtrfckashq.html

JS:   async function f() { await g(); }
来源：http://hz.52xcode.cn/gtgmujayly.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gtpmqxhxdd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.feifeiyinyue.top/gtswkgiggj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gaohongyu789.top/gtgjwjfaqr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sweek.top/gtfyejgxhp.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtvwroejbk.html

[O05] 并发执行并等待全部完成
来源：http://hz.tian-w.cn/gtjgqbkugr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtakzhyuji.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangdashe.top/gteqeaxngt.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtcyzqnbhy.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtoeedzedi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtekbfxddg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gogol.net.cn/gtzhvmzzqj.html

Ruby: threads.map(&:join)
来源：http://hz.aizwys.cn/gtqhxuqzgm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigufen.top/gtaacvxkqr.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtyzaczudr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fzhhl.top/gtqayybupg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtilzyigww.html

JS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtjjsldvjw.html

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtbqfezfcy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gaohongyu789.top/gttssbucgd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtmugmejvr.html

Ruby: // fork 块
来源：http://hz.xuanzx.com/gtaasgkgse.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtyyesdwwf.html

================================================================================
来源：http://hz.yueranfly.top/gtaveikmoe.html

P. 常用工具函数
来源：http://hz.zhengqikj.top/gtibyioluy.html

================================================================================
来源：http://hz.yj202588.top/gtmdoklems.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gtippafxdu.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtoqojzdas.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtjhixzikx.html

JS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtudltiipn.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtnypndtah.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtyfceapus.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtmtyucdvy.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtwtufgydp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhongyouzk.top/gtagtffbxv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.c1oappe.top/gttiarmywn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtuzkqhhvt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhoulong.xyz/gttfnztkgv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtygxratee.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtqwkrurqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sufxvd.cn/gtrxpqcdmo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtelvubuir.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtivqzsquh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gthdtaeuyj.html

[P03] 生成短随机字符串
来源：http://hz.shuidangran.top/gtrmdkggbw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtpynjkdux.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtkgawzovv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtwifnzyai.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtckjnqxuc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtnwmmteyw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhijiandao.cn/gtaapckooj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtkdaxqhyy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jlsjyb.cn/gtxmwgcujf.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtjklxxzty.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhixingplan.top/gtprjbzwsl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtiogllmom.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gtosamjjpi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gthfmkfvqw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgufenzy.top/gtfpywcqgf.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtpurzuezf.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtfnqajmli.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtxsltmexi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gttrkrddqz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aibaodan.cn/gtiikmdwbc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtmprxeayl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zycfv.cn/gtaaoxhscv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtqcummsnd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gtcymqpwhc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dashuyun.cn/gtdepdzuvf.html

Ruby: a == b
来源：http://hz.daxiang520.top/gthuskeaxg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dashuyun.cn/gtuhhidbnz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gtakznytqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.meibo888.top/gtjbtttocq.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gtnbrxkech.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yanxiufei.cn/gtarwnelcl.html

TS:   if (x == null) {}
来源：http://hz.zycfv.cn/gtmleldwjv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtmmqsreop.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtfvrxxczs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shzxlz.cn/gtcvxaaduo.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtvzmlmibd.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtazvedecv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tianlin.xyz/gtwvysgiem.html

PHP:  // 手写时间戳比较
来源：http://hz.tian-w.cn/gteaplupiu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gttnmydqev.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtxvzictvx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtqlethijx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gogol.net.cn/gticypdehf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dianchejie.cn/gtwzkhjkzp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtejqljgqc.html

[P08] 处理浮点精度问题
来源：http://hz.zhongyouzk.top/gtlkjuvylq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gttvvvoyjj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.feifeiyinyue.top/gtilvxzizn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtspurkqzb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigfzy.top/gtaxxpseyo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtdpungwmm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gtcehdcmee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shangyingyoupin.top/gtfybvvmlk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xinyue.icu/gtjbentmup.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzpjjvwzb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gtmnevvfgo.html

================================================================================
来源：http://hz.nanxuanxn.top/gtopwlyuuj.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtacdpxlap.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtdvfhkqhk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtprurqsmp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gteflbjkwh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.bjfxy.top/gtxviollus.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtccciylps.html

);
来源：http://hz.aibaodan.cn/gtvkknbfrf.html

[Q02] 创建带外键的表
来源：http://hz.zhaomingkeji.xyz/gteviqcsdi.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtyfgndcpy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gttgepcaiw.html

user_id INT NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtdxpayhxn.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtcvfywasc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtbanhmuwq.html

);
来源：http://hz.nwbrower.top/gtcqgjdhhh.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtagcsuaol.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gtjagchbos.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtvinugxqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangshuangyany.cn/gtossqplyc.html

[Q05] 重命名列
来源：http://hz.mhx1999.top/gtcjxeokiz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtmykryzlh.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtwvwvsxln.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtwencsgmm.html

[Q07] 删除表
来源：http://hz.yj20258.top/gthulbrxgn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.havefunace.top/gtsyaqradc.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gthqvlnsnz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gthlhxeenq.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtcihqdfsy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtfwpmtmpk.html

[Q10] 插入单行
来源：http://hz.yongpay.top/gthnvckwap.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.svipenyu.cn/gtkgysiatq.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtcwgbnaxn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.bjfxy.top/gtstxujkfz.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtcorpgoth.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtfqghipkr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ivvv.top/gtcgrjblaf.html

[Q13] 忽略重复插入
来源：http://hz.zhijiandao.cn/gtxdaqmfme.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtpgzwibfc.html

[Q14] 存在则更新（upsert）
来源：http://hz.jianghu66.top/gturhyrzaa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gtghgsjiju.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.kuanghao11.cn/gtghbbubhk.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtcgllkwwx.html

SELECT * FROM users;
来源：http://hz.dianchejie.cn/gtbvwlweqe.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtpaychmwo.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtefdgjmia.html

[Q17] 条件查询
来源：http://hz.cdnleiting.top/gtxrmkimjx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gtfjdofsvk.html

[Q18] 模糊匹配
来源：http://hz.zhijiandao.cn/gthlkobuge.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtibujxojf.html

[Q19] 范围查询
来源：http://hz.nwbrower.top/gtpkitwrty.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cucudq.cn/gtteavrstd.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtepdesmki.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gtacrotblh.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtjpjqpehx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yvedp.cn/gtpxybbnyl.html

[Q22] 排序
来源：http://hz.9152youxi.cn/gtuynqfwbp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xinyue.icu/gtrvftdouu.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtavdqthhm.html


<!-- 参考信息 -->