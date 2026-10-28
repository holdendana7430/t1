代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangkeji.top/gtnxznppkt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtwdtmtofp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtqouijcvh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtqcjsdpbj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtzzuwrvio.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtepjbjgig.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtpmeylucx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtctmfzuqo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtndngiktf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gthkqggkbz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtpmjuexul.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.meibo888.top/gtfxkoyhjg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gttumbreii.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtgypkokzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtvyzywafo.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtdwrpgdcq.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtnjsvhomn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gtxutlzmjh.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gtcfbqlxud.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtowzpkvxh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtfjmqfdgf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtnmbjkyzj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtqhlncyvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtpcyhhamm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.9152youxi.cn/gtznbzgexh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ehwqpu.com/gtuwhpyagz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gteqazqzww.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gtbdkaothb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtfchypurm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtfjbxkofg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtnikwifoq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtzmimezcr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxinkj.top/gtoueobedn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtmolhqkbw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtjekvhhxo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtkmiiuvkc.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtyewnfrmx.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gtavqzlqur.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtguilefoe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtdgznrzft.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtxxkhcmil.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dashuyun.cn/gtndocyqqz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtsdzrmsdc.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtmeowzetf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhaomingkeji.xyz/gtmvsvrqas.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangtech.top/gtyqonhxla.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtkerfdmkq.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtbvqlczza.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtvpjgdviu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtfzsvhdps.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gtcxqyqzlq.html

Go:   // 双指针从两端比较
来源：http://hz.mhx1999.top/gthkcaxsjp.html

Ruby: s == s.reverse
来源：http://hz.sufxvd.cn/gtaoirshcx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtsjjudoik.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtdmuewriw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtqnqgmwez.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gtfulwmces.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtjqbsepja.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhoulong.xyz/gtjsqweaej.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtcgiscztt.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtfyamxxub.html

Ruby: // 手写 Hash
来源：http://hz.yj20258.top/gtbgcewubc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gthayapsnh.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtmrbwcbix.html

Py:   itertools.permutations(arr)
来源：http://hz.smart0.xyz/gtahbqezyn.html

PHP:  // 手写递归交换
来源：http://hz.ivvv.top/gtantgceqc.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtpfztjzwc.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtalqefxas.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gthdgdkpps.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtpfkoxbws.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258.top/gtugylvpcx.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtzivwbdnv.html

[N09] 栈与队列
来源：http://hz.tanke756.top/gtjirmgchi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuanzhike.top/gtdxcqgpvm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtirtnhcex.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtrgsehfsp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuanzx.com/gtpjvspanm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cqqwz.cn/gtudfbbhlm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gthjcpprns.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aizwys.cn/gtgeswmwug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtjuainzre.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtrefaofez.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.snrcjt.cn/gtvywdrvxs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yueranfly.top/gtowfgxbek.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhoulong.xyz/gtlfwrfuqg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtipsijxdz.html

Java: class Node { int v; Node next; }
来源：http://hz.svipenyu.cn/gtzojgzhgx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jiagoushi.top/gtazgwhnhe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtwawqhkbn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtxqifstgt.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtqtjjbprj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtmbyarzpi.html

PHP:  // 手写递归函数
来源：http://hz.zhongyouzk.top/gtlhxyxbfi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtqirkhnqg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtszgnmpoi.html

Java: // 手写递归
来源：http://hz.yuxming.cn/gtxvulvrne.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gtnozdftls.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtzrfjlmxv.html

C#:   // 手写递归
来源：http://hz.dianchejie.cn/gtedlhaipp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ybcxt.top/gtsgpnjsdp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenjidiqi.icu/gtzmotbokn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtafxwqoti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtpzpehbqi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtvmfewdwu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtyzturnsv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtdjbgefxy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ywan-chungtsiang.top/gtoadcnirz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtqovwkcxn.html

================================================================================
来源：http://hz.havefunace.top/gtbcalicpy.html

O. 并发与异步
来源：http://hz.daria6918.cn/gtxkeszdai.html

================================================================================
来源：http://hz.aibaodan.cn/gtraoqwgbr.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtjnuoglxy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gteyuseqfe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtiskuskox.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gttosczadc.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtfvboajat.html

Java: new Thread(() -> f()).start()
来源：http://hz.snrcjt.cn/gtxkoocikl.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtxgrneehy.html

Ruby: Thread.new { f }
来源：http://hz.daxiang520.top/gtlupddfhc.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtuadjehog.html

[O02] 使用线程池
来源：http://hz.xingfuxueyuan.xyz/gtwjsvsvmb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtwgzkhtrl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangkeji.top/gthyuhrwax.html

JS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtgqizcfca.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtvqdszgqp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yueranfly.top/gtmcqpapcm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenzaomai.com/gtovwqzzfx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtmkegdlow.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtlgmszwik.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gtzwjrbvuq.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtcqfygdlg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtluvupzog.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtrbkfyuto.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtpujwzyud.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtkqoviwuv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtvucyfiwv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtihudsykr.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydzc1.top/gtigiojmkc.html

[O04] 定义异步函数并等待
来源：http://hz.smart0.xyz/gtmzzygnvk.html

Py:   async def f():⏎    await g()
来源：http://hz.tanke756.top/gtxwfddtsl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxuanxn.top/gtjbtkowmo.html

JS:   async function f() { await g(); }
来源：http://hz.jinqigfzy.top/gtnalofplc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gtzggrmzmf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtumqkvpzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ybcxt.top/gtrllrbbrb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydjk.org.cn/gtqxavjzyy.html

C#:   async Task F() { await G(); }
来源：http://hz.dashuyun.cn/gtvuxhpuda.html

[O05] 并发执行并等待全部完成
来源：http://hz.xylfe.cn/gtvfaxwiar.html

Py:   asyncio.gather(*tasks)
来源：http://hz.birdmap.top/gtpvyyvpwu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtsysjgneh.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtyzfyztkf.html

TS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtfibvfyvv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hongshengwenyu.top/gtatudctwg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yonumen.top/gttukzidhr.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtcyxcybnr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yvedp.cn/gtanczkkbg.html

[O06] 使用进程池
来源：http://hz.gogol.net.cn/gtoqmknuvr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shzxlz.cn/gthlbwsxgu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cucudq.cn/gtlfhtaryo.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtuwftmqzf.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtnhdxcgce.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtendvnczs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yvedp.cn/gtipvfmxze.html

Ruby: // fork 块
来源：http://hz.xuanzx.com/gtbrlxhiex.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtnujxxcft.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtscfpdaoo.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtolkxdcas.html

================================================================================
来源：http://hz.sweek.top/gtvplkfshn.html

[P01] 生成 UUID
来源：http://hz.bjfxy.top/gtilwseryo.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtwqmzabfc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yangfankeji.com/gtwrruqwbg.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gthatrhckz.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtweglwszt.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtkrhqozvy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tian-w.cn/gtgzhwapwp.html

Ruby: SecureRandom.uuid
来源：http://hz.sysykeji.top/gtndupyfxf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ppjwa.cn/gtmmpvvwtc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtaauvywlb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuetiantiany.cn/gtrbzhwntc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinyuanbaomall.cn/gtnyrsrslb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtjkszjrmm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtdyipplrz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtigppmybz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnxiangtu.top/gtzefmxsxj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gtujmqlmxa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtztjbmywt.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtgmtkvknp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtekzaanil.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gtlymhwbtq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtcoixognz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtcbevrbbk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinyuanbaomall.cn/gtxmgzphwj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtgjqjggev.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtppszxenm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangshuangyany.cn/gtahyfwliz.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtdrwhqqdn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhaomingkeji.xyz/gtiiufkxsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gthuykhcyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtwouviope.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gttladpvpl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtwejuzryf.html

Go:   len(arr);  len(m)
来源：http://hz.yangfankeji.com/gtlljmkhhc.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtdsacbqjb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gteayahsmy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtbfswhgjf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtyhosujbv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.smart0.xyz/gtweyjopha.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.vqdsnc.cn/gtgqopzazt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtukwqnzfm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtkrsyqmrz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtdyrjcgrv.html

Ruby: a == b
来源：http://hz.yvedp.cn/gtnmcnothj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ybcxt.top/gtbjboqoxa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtdrcoqqqx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtwoxdudkh.html

PHP:  if (empty($x)) {}
来源：http://hz.chenlongwang.top/gtvfnyvjci.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daria6918.cn/gtidsmgesd.html

TS:   if (x == null) {}
来源：http://hz.hnqzz.top/gtbjuxofwk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.316326.xyz/gtlzbmdncw.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gtfklhepxo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ivvv.top/gtvprbtplz.html

C#:   if (x is null) {}
来源：http://hz.xuanzx.com/gtzwrdnhmw.html

[P07] 防抖与节流
来源：http://hz.chenlongwang.top/gtplzqiesx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gtnohosbps.html

PHP:  // 手写时间戳比较
来源：http://hz.sysykeji.top/gttgtcwgyl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtvnfhmver.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtwaapdotb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gzhubu.top/gtpmzvdxoi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhijiandao.cn/gtzsekechc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cdnleiting.top/gtbcxhazjo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtcfgsxzpn.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtfauwwuac.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gtllwlxknj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuetiantiany.cn/gteuhklocr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yonumen.top/gtdekbbfid.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.andypj.xyz/gtqitwcdhp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtfbggjxfs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtivmoxssx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gtatpvujdi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtxnyvkjjt.html

================================================================================
来源：http://hz.hammf.cn/gtqbcoemns.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hysaishi.cn/gtmprrlmph.html

================================================================================
来源：http://hz.andypj.xyz/gtqcdeexon.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtqizmroxf.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtftiicvlg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtfkmtkcjt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.316326.xyz/gtoxngnuhs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gtwdjsfnaq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtwkdkrqwb.html

);
来源：http://hz.gotoacloud.top/gtorcbqyan.html

[Q02] 创建带外键的表
来源：http://hz.haohaochexian.top/gtaxegmsnn.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gthulzdnnm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtkibpejsp.html

user_id INT NOT NULL,
来源：http://hz.iojbl.cn/gtqudjjulq.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtgzfwrsex.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guannengcc.top/gtbizproya.html

);
来源：http://hz.snrcjt.cn/gttrqkosmc.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtsthraogz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtblutcyxu.html

[Q04] 修改列类型
来源：http://hz.feifeiyinyue.top/gtefevrdji.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtlecqcmod.html

[Q05] 重命名列
来源：http://hz.xuanzx.com/gtkyxugugd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtdtqugoqy.html

[Q06] 删除列
来源：http://hz.shuidangran.top/gtlsamszwk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xingfuxueyuan.xyz/gtfgztuaxs.html

[Q07] 删除表
来源：http://hz.0kj1m.cn/gtbtwivcya.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtzetcxhfp.html

[Q08] 创建普通索引
来源：http://hz.xylfe.cn/gtmpoeebhe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtvxuupxpf.html

[Q09] 创建唯一索引
来源：http://hz.jinqigfzy.top/gtkdoduugr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtpwcpumie.html

[Q10] 插入单行
来源：http://hz.jinghuilouyu.cn/gtwbnosjfj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gtfjjfnyvd.html

[Q11] 一次插入多行
来源：http://hz.ywan-chungtsiang.top/gthehomaeh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtsmguumcv.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtsyewknjv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fengsongda.top/gtzvmrgzhe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtfyvywamm.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtwvwnkpza.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtobmsrflw.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangshuangyany.cn/gtiygcciem.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gthvpvsydj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.dashuyun.cn/gtgaoisbcd.html

[Q15] 查询全部
来源：http://hz.yongpay.top/gtfftsvctj.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtzddjxwdu.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangtech.top/gtkrvhfpfe.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtvckeuldh.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtjqyaospz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.kuanghao11.cn/gtqwtrylef.html

[Q18] 模糊匹配
来源：http://hz.cheryme.top/gtyyartxxd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gtodexopdn.html

[Q19] 范围查询
来源：http://hz.shanyushiyangtech.top/gtuffdpqfw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hongshengwenyu.top/gtysyihmuw.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtnuhrxjff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtlooishze.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gtvngolswf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cucudq.cn/gtkctllcsx.html

[Q22] 排序
来源：http://hz.zycfv.cn/gtwdrihkxt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gtalzndbbu.html

[Q23] 分页
来源：http://hz.316326.xyz/gtpkcurqan.html


<!-- 参考信息 -->