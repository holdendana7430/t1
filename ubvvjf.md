代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtzqbqdmid.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtcwttwxkv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yanxiufei.cn/gtnsioyljs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.haohaochexian.top/gtvyxaitty.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yvedp.cn/gtihoufkaw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtqbdeemzg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtnvbybbav.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtqpanetla.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtprtgkyhy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtlypvdizd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shuidangran.top/gtwvfqrvlm.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtruhvevyk.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtfixtofqw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.0kj1m.cn/gtppgowabl.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtcmrrtaho.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtqctruyol.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtdiapzbzi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtsuocxemf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtcxhbconj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gttljfklbv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sufxvd.cn/gtypmuolhl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtiorbklbz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cheryme.top/gtwvwgampb.html

[N04] 斐波那契数列
来源：http://hz.nanxinkj.top/gtyeccibxi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtqevsrnwm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtorrjdndy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtgpeowvvh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtoctfglry.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtozlqgaet.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gtpolmsknv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtmleihkxp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtkxgtdnyz.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtpsvsvzhm.html

Py:   math.gcd(a, b)
来源：http://hz.xylfe.cn/gtvzpdkntw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtpllvetkn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtipslbdcp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtwnpkdrht.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtffoijgaj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aibaodan.cn/gthtoboafx.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtqhgymuvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sweek.top/gtfrakzrud.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gttrvpvmxs.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gtvcvotlhi.html

PHP:  $s === strrev($s);
来源：http://hz.cucudq.cn/gtjcascdsl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtraplwmhe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtkvspppew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtxmqegqpc.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtxhqlibpl.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtglukiilq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtbmqnfycb.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtvuhdyecj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtcbposrfu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtbekmmgfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtuqobxwzw.html

TS:   // 手写 Map<string, number>
来源：http://hz.jiagoushi.top/gtdlrrxlyf.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtutcgxtzp.html

Go:   // 手写 map[int]int
来源：http://hz.ivvv.top/gtecyeagad.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtrnhwvjun.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtaiunpsbb.html

[N08] 生成全排列
来源：http://hz.jinghuilouyu.cn/gtfaokaleg.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtvsnbftmv.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtrpbghltq.html

JS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtwmnjxpua.html

TS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtufmrmmny.html

Java: // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtqkovphxi.html

Go:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtwrjpnuvw.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtzctxorsh.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtizajfjeb.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtlrqvybta.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtqlxjiqee.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtogotbdzv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gtlsuefppx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guannengcc.top/gtblpuasqq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtyaejcudu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtoxdquswp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gttuphlwxu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.iojbl.cn/gtjjgzgdmk.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtyyjlccka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.andypj.xyz/gtqfjkkmvd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhixingplan.top/gtvbhzjfcm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gteigjhvlf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gogol.net.cn/gttordnmjr.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtlncjpkkv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtqwtzfgzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj202588.top/gtyxobmznu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gtyvtjzugc.html

[N11] 二叉树中序遍历
来源：http://hz.zdqjudy.top/gtwjovvxxr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtryfcztsp.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtmynjlebx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtdzrrcrkr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtlyzkdzuh.html

Java: // 手写递归
来源：http://hz.cdnleiting.top/gtvvrmukzk.html

Go:   // 手写递归
来源：http://hz.vqdsnc.cn/gtlxurvgbv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtjvzfiuvi.html

C#:   // 手写递归
来源：http://hz.jlsjyb.cn/gtlgeyliat.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtffmtkzsw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtgzrqfjcs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtnvblfsdf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtiuaadmjr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtvzrqrzdq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gtwtbhjacm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtttdxgcwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cheryme.top/gtjqoqspkq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gtksvrmpmc.html

================================================================================
来源：http://hz.ydjk.org.cn/gttrwfyywi.html

O. 并发与异步
来源：http://hz.zhijiandao.cn/gtapudzodh.html

================================================================================
来源：http://hz.yueranfly.top/gttxdrxiaa.html

[O01] 启动一个线程
来源：http://hz.hammf.cn/gtxfrgzhxz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hongshengwenyu.top/gtduhylrxn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gzhubu.top/gtvmawtsjw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtporphboa.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtdpvjhnvj.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtxzbxgyqs.html

Go:   go f()
来源：http://hz.jinqigufen.top/gtspswrzww.html

Ruby: Thread.new { f }
来源：http://hz.yvedp.cn/gtljrdxwbp.html

C#:   Task.Run(() => F());
来源：http://hz.cashguo.top/gtasqimyti.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtaxkiqcke.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtjvucxehm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtqhvcbopf.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtrtpetbnq.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gthbalnrrz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtuvjkilmv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtztpsslfo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtxzfpwbpv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtwojdsxdr.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangkeji.top/gtljzwcfnh.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtjooqvkhv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtywpcztqv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gtacsadfbz.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtixrrfxbc.html

Java: synchronized (this) { shared++; }
来源：http://hz.cheryme.top/gtibzygnam.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtlgqpephb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gtpmtbtjso.html

C#:   lock (gate) { shared++; }
来源：http://hz.yonumen.top/gtmmuukbyp.html

[O04] 定义异步函数并等待
来源：http://hz.shuidangran.top/gtynhipcai.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gttkklxrnt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtfgmzsndk.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gtlrhexxrq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuanzhike.top/gtvszycwrr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangtech.top/gtaicijkco.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuetiantiany.cn/gtumlzuqtd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ybcxt.top/gttjpvcokv.html

C#:   async Task F() { await G(); }
来源：http://hz.redwolf501.top/gtjcunamda.html

[O05] 并发执行并等待全部完成
来源：http://hz.guannengcc.top/gttzpvwvtm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinghuilouyu.cn/gtkbrswbqz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.birdmap.top/gtqekrqbxo.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtuswebakm.html

TS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtybgsokwg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtxdivlagi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.mhx1999.top/gtrnfxblys.html

Ruby: threads.map(&:join)
来源：http://hz.zycfv.cn/gtvdqqjhil.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.smart0.xyz/gtekujflvo.html

[O06] 使用进程池
来源：http://hz.9152youxi.cn/gtsuxbukhe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtkdgwwgxv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtpimmcaqw.html

JS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtrdozsnxy.html

TS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gthrtkdjzp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtwggttmyj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtkzszwjxj.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtlzbxdqsc.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtjdqsdvkn.html

================================================================================
来源：http://hz.dashuyun.cn/gtlzrlmujm.html

P. 常用工具函数
来源：http://hz.fzhhl.top/gtzsglnoko.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxwzimuma.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtsexfqrre.html

Py:   str(uuid.uuid4())
来源：http://hz.yangfankeji.com/gtlvxqctzm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtlyzidkhs.html

JS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtbrankgvy.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtshbbxuxt.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtqmnjfchu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.snrcjt.cn/gtkqzebleu.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtjhpigilu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhengqikj.top/gtuitpteqd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtsxtcedkf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtpaubrdui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenjidiqi.icu/gtdsrgqgld.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtqrnutlgs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daria6918.cn/gtdhasmthl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtyolzrlcs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnqzz.top/gtkkgtujtw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dianchejie.cn/gtthbvcadv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gotoacloud.top/gtzuuadnqw.html

[P03] 生成短随机字符串
来源：http://hz.yongpay.top/gtuzdvfbrz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dianchejie.cn/gtgrclyuvm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.vqdsnc.cn/gtpfhuccxv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtiamycqer.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtvjzwaayb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtrjcrfjpl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtzwrqzfyt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.birdmap.top/gtmpmcbzen.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aibaodan.cn/gtgvquasna.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtteipgvwb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtldlifokk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtlnrrbtue.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtbcgznmte.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtjikgthfj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtbhhthkiw.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangkeji.top/gthemcivgr.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtcuulfldm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sufxvd.cn/gthwwjtezp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhaomingkeji.xyz/gtihmkoucz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.9152youxi.cn/gttaizjvpl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jiagoushi.top/gtdilwsfxn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtdfqxikev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtqiowspod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gaohongyu789.top/gtzvgplllm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtlafrugbp.html

Ruby: a == b
来源：http://hz.gogol.net.cn/gtrbhbitkr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.316326.xyz/gtvlyxmuig.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guowangkeji.top/gtxwqzfgjx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtztjfnced.html

PHP:  if (empty($x)) {}
来源：http://hz.quarkkingdee.top/gtdtyvuftc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yanxiufei.cn/gtpojtchqp.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gtlupeoyls.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtrcmpvwjs.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtnrfranri.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pycfn.com/gtybvsxqef.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtvmtlljac.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gtirexqvyo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ywan-chungtsiang.top/gtpvlzttxd.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtfsvdbzdn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtphweytpl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtmcvnkvuv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhiwuduotai.top/gtstnglntp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yueranfly.top/gtruevrevr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hfpthk.cn/gttpktdcvr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tianlin.xyz/gtnpzpxoig.html

[P08] 处理浮点精度问题
来源：http://hz.jinyuanbaomall.cn/gtmyxpjhvd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtpunqmihc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gterhkshuq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtuhvkvlxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gtexvcsgtg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtwpvaszbd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gthjvvsqij.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtyoqpuutg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.9152youxi.cn/gtyrqjpyuv.html

================================================================================
来源：http://hz.jyoumei.cn/gtgfljtqlw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cdnleiting.top/gtvorraaii.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtfrmulxpt.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtazyvwmpc.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtlkjmnzle.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtodrdlqqt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgfzy.top/gtdzvbwugc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtnperxrht.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhiwuduotai.top/gtiejyhthj.html

);
来源：http://hz.nanxinkj.top/gtcwqyrfxp.html

[Q02] 创建带外键的表
来源：http://hz.dianchejie.cn/gtugbltghm.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtygyrjvuz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtyhcprxyi.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtjpiqigyf.html

amount DECIMAL(10, 2),
来源：http://hz.hnqzz.top/gtonzgrjzr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtekrvrbob.html

);
来源：http://hz.jqgufenzy.top/gtdliiqjdu.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtnlhrrjyx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gtkegkgsaz.html

[Q04] 修改列类型
来源：http://hz.yuanzhike.top/gtviqqystu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ivvv.top/gththhvjrb.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtffrhsncu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtieynyvrh.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gteulfnmeb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtvnurxgfv.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gttqmdgwpp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtyplwuiov.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gtvssnyjkl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtdjlrktpn.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtxpgjirnd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtqidyrudg.html

[Q10] 插入单行
来源：http://hz.snrcjt.cn/gtintqbrrd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtwkczieyq.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtxzucxkmf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtiaxytjvs.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gterbckpyg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtdbqptvcj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtqzerwabw.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtielmgjrs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gtgxajclup.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gttgrmtwhn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gtacucsxnu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgufenzy.top/gtsakhgkar.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtabcijldl.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtbhbvtchc.html

[Q16] 查询指定列
来源：http://hz.xziqi.cn/gtastrnimw.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwdvzwvsz.html

[Q17] 条件查询
来源：http://hz.xuetiantiany.cn/gttjkljume.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtdioudruv.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtoyhbfyyp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtjzvpwete.html

[Q19] 范围查询
来源：http://hz.shzxlz.cn/gttepvncms.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shuidangran.top/gtmgklkszs.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtbqzoqokd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtjcjbaxqu.html

[Q21] 空值判断
来源：http://hz.dianchejie.cn/gtgvwimwyu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zdqjudy.top/gtxusjbswa.html

[Q22] 排序
来源：http://hz.gotoacloud.top/gtonjzqkvb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtxuoldsux.html

[Q23] 分页
来源：http://hz.gzhubu.top/gtvfnznefw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gtnoxseeiq.html

[Q24] 去重
来源：http://hz.zycfv.cn/gtpsrtiyxb.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gtqvljkkvi.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangtech.top/gtydzhbcud.html


<!-- 参考信息 -->