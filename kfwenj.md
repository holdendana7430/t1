代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtchxdrsmr.html

================================================================================
来源：http://hz.dianchejie.cn/gtdghupyrj.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gtsovzvahk.html

================================================================================
来源：http://hz.xziqi.cn/gthsyvrdaj.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtqnocvoqk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenjidiqi.icu/gtrszgunlu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtdqfeqfax.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtqtrjlnox.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtekbctqbl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtqjgsowqv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtbzohrmie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.316326.xyz/gtmzqxzhxl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtfntyprcb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtgybydgnm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gttebqokkl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gtabsoittl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtrwbznnnu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtyhqaariq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gtgztikwkn.html

Go:   slices.Sort(arr)
来源：http://hz.pycfn.com/gtgpersozs.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtptwtqacd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtirlcuzwe.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtvrxpgcpz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gttgrtmnag.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtbhyxzmug.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtnufvecna.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gthvxaxlio.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtbdeblmuz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenjidiqi.icu/gtlmoriltd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258888.top/gtgkjwkmxh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigufen.top/gtrwctqjaz.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtmnigeyia.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gtvjqjvrst.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fzhhl.top/gtgioyavjm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtfawvlque.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtsznnyutf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtjquycckh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtytpadiaj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtftrfqoda.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtwoxakuzu.html

[N05] 最大公约数
来源：http://hz.zhiwuduotai.top/gtqdbelwuq.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtyyneobom.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daxiang520.top/gtxvvdydxy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtdfcszqoz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtfegwauux.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtalkqjihm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxinkj.top/gtgymnvgej.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangtech.top/gtixqosrym.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.meibo888.top/gttwkwuvry.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtjktccksc.html

Py:   s == s[::-1]
来源：http://hz.zycfv.cn/gtgomgibpg.html

PHP:  $s === strrev($s);
来源：http://hz.gogol.net.cn/gtzagecxpn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtlsmtxzsi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtcitxbcwb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gttizntwrc.html

Go:   // 双指针从两端比较
来源：http://hz.dashuyun.cn/gtdkhazfwz.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gtrcpsqlnl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtawdephmw.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtdvtorgip.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtqiegbfrh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gthemynbmp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aibaodan.cn/gtukhbiaaz.html

TS:   // 手写 Map<string, number>
来源：http://hz.gogol.net.cn/gtvuzbikyu.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtdldobwnc.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtwjyxyfzq.html

Ruby: // 手写 Hash
来源：http://hz.ybcxt.top/gtnqpbcnkx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtkndknnfz.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gtysilxjby.html

Py:   itertools.permutations(arr)
来源：http://hz.ehwqpu.com/gtdrzrjnxt.html

PHP:  // 手写递归交换
来源：http://hz.cheryme.top/gteivtbnzq.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtxqyluius.html

TS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtxqaltwpw.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtexdeuvkw.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gticvoidqq.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gthmzfpzsm.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtfkkjhecw.html

[N09] 栈与队列
来源：http://hz.cqqwz.cn/gthsdlkoin.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.52xcode.cn/gtyxskghbu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gotoacloud.top/gtrwjxkaxu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtplnmcpal.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hysaishi.cn/gtdcnkrdkw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtajmyamlo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gttqpliqpv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yonumen.top/gtilwncdei.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gtfczbgvfw.html

[N10] 链表节点定义
来源：http://hz.chenlongwang.top/gtijhmiecc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhaomingkeji.xyz/gtsmdkcupx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuanzx.com/gtxzvcdyjn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dianchejie.cn/gtpscdrgzi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtdndwavrs.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtviajikfg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.vqdsnc.cn/gtxuiyxelu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtikbtpacd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hysaishi.cn/gtresenxaq.html

[N11] 二叉树中序遍历
来源：http://hz.meibo888.top/gtvhqnydqk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydzc1.top/gtcptflutt.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtpvqjvgvz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gttfskmvgo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtlmpvnnar.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtbamyfoht.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtugxvuhmy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtiflajrag.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtxvnluwme.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtomexhell.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gtdfrvkmql.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtmpmpcuyv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtosvpsgcj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtotguzyvv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtsixctymh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fengsongda.top/gttswbyoaj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sweek.top/gtwzifdkda.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtcbinoxrd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtoscckltd.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtanbzhlem.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtltqjpbbo.html

[O01] 启动一个线程
来源：http://hz.zycfv.cn/gttvpljgom.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xylfe.cn/gtmifnarsx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtdwvlclvv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtgkkyxfmd.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gterwrgvpg.html

Java: new Thread(() -> f()).start()
来源：http://hz.ppjwa.cn/gtlybbdodr.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtjvjgzxkb.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gttaenzkpb.html

C#:   Task.Run(() => F());
来源：http://hz.gogol.net.cn/gtcsunkwjt.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtnfywaxgq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yongpay.top/gthnonvysf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tanke756.top/gtutrnirdc.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtqwqysahk.html

TS:   // worker_threads 线程池
来源：http://hz.zhengqikj.top/gtavrbsyth.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtthcemime.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtciyeqbjz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fengsongda.top/gtgrzuwxjd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenlongwang.top/gtwijhawpt.html

[O03] 加锁保护共享数据
来源：http://hz.meibo888.top/gtdmoqjksh.html

Py:   with lock: shared += 1
来源：http://hz.shuidangran.top/gtvcsvceuh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtskxhnkbr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gtbxutxozc.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtfjuxmddb.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtgwqycgqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gtfztqulhi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtndfdevws.html

C#:   lock (gate) { shared++; }
来源：http://hz.andypj.xyz/gtdmowdbar.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtwfmhdyax.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtptbqpjzu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtcbsnhizn.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtimrkirdx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hammf.cn/gtibrmethu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gogol.net.cn/gtfczeiysm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtnzdtpddg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhixingplan.top/gtodtphegw.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtjpkuhzya.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtnwoaoyqh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtoduemszf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydjk.org.cn/gtzqfebich.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtrsellzna.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtxfgxdmsj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtvofajrtq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.andypj.xyz/gtxhtepgyd.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtqwseucuc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtwbdzqivt.html

[O06] 使用进程池
来源：http://hz.yj20258.top/gtkmiwinar.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtmqdsmwtl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtnregldfl.html

JS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtsokpaidj.html

TS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtwjmtyfnt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aizwys.cn/gtvsplrwje.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gtjibrbqfj.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gtemkjcodz.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtwnpaecrw.html

================================================================================
来源：http://hz.jianghu66.top/gtuqmtitdl.html

P. 常用工具函数
来源：http://hz.jianghu66.top/gtjcislskh.html

================================================================================
来源：http://hz.pycfn.com/gtvgprxkms.html

[P01] 生成 UUID
来源：http://hz.yj20258.top/gtreqanawu.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtlhmtewcz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxuanxn.top/gtqejkwudk.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtljvncqoy.html

TS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtdhurnafv.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtqmqslbpm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.haohaochexian.top/gtlgvjfmma.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtyqgfmcjs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuxming.cn/gtmsjcmlnj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenlongwang.top/gtltjswvue.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgfzy.top/gthnidfkhd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtlhsvwhsf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gtgrcredxk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtesovlqpp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gteilwegig.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangshuangyany.cn/gtusxagrho.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtvskgcnin.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.iojbl.cn/gtuoyzldqt.html

[P03] 生成短随机字符串
来源：http://hz.zhaomingkeji.xyz/gtsoofpwas.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gthpnnsvru.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.mhx1999.top/gtzmeypnoi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtsezzxzxm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtzrbubfkr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtkftoaphw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cheryme.top/gtbdxcvckt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydzc1.top/gtbseveflv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuetiantiany.cn/gtsnckjllw.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtsheszhjv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtnfeelzdp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtofocajld.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtnmtnmvxq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtmqucoyof.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtggqfkztu.html

Go:   len(arr);  len(m)
来源：http://hz.hnxiangtu.top/gtmayuwqfr.html

Ruby: x.length;  x.size
来源：http://hz.dashuyun.cn/gttaavcujl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sufxvd.cn/gtcxxfvdwb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hywenlv.cn/gtjtzwdtjw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zycfv.cn/gtkribgvbq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhoulong.xyz/gtptwlmxln.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtyhyeafff.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtnxlcrseb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhoulong.xyz/gtvecfnbfz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtygvsuhaq.html

Ruby: a == b
来源：http://hz.jyoumei.cn/gtbuorgrbp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gttpztqnpm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtpbbvkqob.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtiiwnrsgc.html

PHP:  if (empty($x)) {}
来源：http://hz.wangshuangyany.cn/gtvqdfscsp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtjynynest.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gttupbxfhn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuxming.cn/gtupzonjkp.html

Go:   if x == nil {}
来源：http://hz.wangdashe.top/gtbkazlfhl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zycfv.cn/gtgvzcfoax.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gtotktvakm.html

[P07] 防抖与节流
来源：http://hz.cqqwz.cn/gtadfehkkw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtupihcliw.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gtdwvtvwig.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtosupmmud.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtfuczfsfw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gtboyyzkrs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gtymxenlcp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangkeji.top/gtsiubberw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hammf.cn/gtmqosowyj.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtqmhlbgzt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dianchejie.cn/gtpwoqnpft.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgfzy.top/gtrzsirbxx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtrbwjcemx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ybcxt.top/gtnurfwlxj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yvedp.cn/gtjuagvkto.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtyjjgvhql.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtjrqxkudr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtgqbfupmo.html

================================================================================
来源：http://hz.yj20258888.top/gtosxloond.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtnjpllkye.html

================================================================================
来源：http://hz.meibo888.top/gttipwardl.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtsrmembgf.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtixonbnhs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gtmaltyayj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gtraraqnsq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gtnberikjl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtajtkndip.html

);
来源：http://hz.cashguo.top/gtbsjrdtmm.html

[Q02] 创建带外键的表
来源：http://hz.gaohongyu789.top/gtjkwzdjoc.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtqxeevlcs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtlpngufat.html

user_id INT NOT NULL,
来源：http://hz.nanxuanxn.top/gtplryklxc.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gteakqjsuk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tian-w.cn/gtxvlrfrjf.html

);
来源：http://hz.jinyuanbaomall.cn/gtqkviobbd.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtykjrutbm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258.top/gtvqgmppzb.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtqldpomve.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtzekepcei.html

[Q05] 重命名列
来源：http://hz.sufxvd.cn/gtnneyiqbi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yvedp.cn/gtozshegij.html

[Q06] 删除列
来源：http://hz.yj20258.top/gtkelzwxvu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtmnofrghm.html

[Q07] 删除表
来源：http://hz.ppjwa.cn/gtwoolktpq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhongyouzk.top/gtxdblkwuq.html

[Q08] 创建普通索引
来源：http://hz.jinqigfzy.top/gtlninsekz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtcqqxdkgc.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gtmboexgyf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtroezjxwy.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtuzelszqg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gtmqzmrsyk.html

[Q11] 一次插入多行
来源：http://hz.shzxlz.cn/gtpmxspzau.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtryqhvuls.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtaduboben.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtyfpvdbay.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jiagoushi.top/gtxboniauz.html

[Q13] 忽略重复插入
来源：http://hz.xziqi.cn/gtbffnywab.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtsleeowks.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtdqkwmlnz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.0kj1m.cn/gtefezifok.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gttxuybgyx.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtzkodauhi.html

SELECT * FROM users;
来源：http://hz.iojbl.cn/gtrnmxwlil.html

[Q16] 查询指定列
来源：http://hz.gaohongyu789.top/gturbztlnb.html

SELECT id, name FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtfwarfwxv.html

[Q17] 条件查询
来源：http://hz.hfpthk.cn/gtlqmlwbgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gtipsmkzik.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtgkjkqvyw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.vqdsnc.cn/gtkschnozr.html

[Q19] 范围查询
来源：http://hz.cucudq.cn/gthubhypuq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guowangkeji.top/gtanbuhawj.html

[Q20] IN 列表
来源：http://hz.shuidangran.top/gtwkvismoa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydzc1.top/gtfjlbxcvl.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtrpsmzsze.html


<!-- 参考信息 -->