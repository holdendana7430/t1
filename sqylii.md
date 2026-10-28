代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gttrveskds.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtrdioyhhj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtesuutdbi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gogol.net.cn/gtvkfnxugx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtlxrttjmq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gttjjwwplm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtglplrdof.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gtraegprkc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gttvqitsfa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtpyvkzebp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtczvcbesv.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtmiqlambn.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtfaggwgik.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fzhhl.top/gtqfidyzix.html

[N03] 快速排序（分治示例）
来源：http://hz.shuidangran.top/gtxibbisub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gtxfftvwwu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aizwys.cn/gtsdjckplp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtzhxqpeab.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gthslmksag.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtacvcyvdo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hammf.cn/gtvavqflfi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtdfdstcac.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtjhdtjmmc.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtrfiodlgp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtfxxhegoo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.pycfn.com/gthgocldjb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gtjaqazvjk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtnfuuimdb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hammf.cn/gtznwiyxho.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtdknkovle.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtqtivmeuo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtofcgsyyr.html

[N05] 最大公约数
来源：http://hz.zhengqikj.top/gtprivdbwy.html

Py:   math.gcd(a, b)
来源：http://hz.zhengqikj.top/gtjajosuqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xingfuxueyuan.xyz/gtxfejpeep.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtwsmuaymm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtgsughklq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fengsongda.top/gtidykfwrv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangdashe.top/gtvozwjgas.html

Ruby: a.gcd(b)
来源：http://hz.nwbrower.top/gtyaqrdyfy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.daxiang520.top/gtknwvcibk.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtsxfytatz.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtbqllxdmj.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gtpdfpcvzm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtghzkfmeb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtvvynugho.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtetpeoghn.html

Go:   // 双指针从两端比较
来源：http://hz.cdnleiting.top/gtaswjgrlk.html

Ruby: s == s.reverse
来源：http://hz.pycfn.com/gtqpbtiphp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtdtgxayas.html

[N07] 两数之和（返回下标）
来源：http://hz.tianlin.xyz/gtpqppjqzh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtukwsjrfs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gthufrejsx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtvtgfgmyi.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtpssmehzo.html

Java: // 手写 HashMap
来源：http://hz.ybcxt.top/gtbjlebfqd.html

Go:   // 手写 map[int]int
来源：http://hz.yangfankeji.com/gtefrusysn.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtpsteocvl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtymehmknd.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtjzkcdrei.html

Py:   itertools.permutations(arr)
来源：http://hz.hysaishi.cn/gtosullpae.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtanbezulj.html

JS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtlehrditj.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtstsuhnhw.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtiihboxan.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtkeiijvns.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtcoccyolx.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtaarejeck.html

[N09] 栈与队列
来源：http://hz.svipenyu.cn/gtbqhtbybj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yanxiufei.cn/gtzeeybmxx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydjk.org.cn/gthuatfxwy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtrexysjia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuxming.cn/gteehuqevt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtvofuylyh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gtzufvvwjd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtyqqchvme.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtzpclddlo.html

[N10] 链表节点定义
来源：http://hz.zhongyouzk.top/gtytxqetyt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtpmpghrjt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhiwuduotai.top/gtpqvtwawk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigfzy.top/gtswyxzzic.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtxgsoufje.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtksfrycjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtcufxhbjo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenjidiqi.icu/gtxpciwldv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xinyue.icu/gtvdeluucq.html

[N11] 二叉树中序遍历
来源：http://hz.andypj.xyz/gtkqieaadc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtqvteeuww.html

PHP:  // 手写递归函数
来源：http://hz.yuanzhike.top/gtfznvgtfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtrxphreis.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtggiqdfsh.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtchrcqdlc.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtsmjtasgl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtooosiirr.html

C#:   // 手写递归
来源：http://hz.andypj.xyz/gtkvptijca.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtlrvvxlby.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.birdmap.top/gtrqlomymz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtigfdpsdf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtrekxygha.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtocskskhe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtnnzrxghv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gzhubu.top/gtiswbrjpr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gtlweswdhq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtlgjhgjlv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtofyxxpul.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtvxmasgfd.html

================================================================================
来源：http://hz.yueranfly.top/gttvxsiieh.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtvnyoixdf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tanke756.top/gtfmmdmobl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtyatpqzju.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aibaodan.cn/gtsxfgbmzx.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtohkwmqjo.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtomxksvxi.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtrfxbdmal.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtxyamdwbg.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtxiiproin.html

[O02] 使用线程池
来源：http://hz.nwbrower.top/gtvczdnwtx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ybcxt.top/gthfagdmpe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sufxvd.cn/gtycxntkzu.html

JS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gtkziezmfw.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtjxrznele.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtvscaicne.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtzewyyofh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guannengcc.top/gtjjevadpg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gzhubu.top/gtdikeqvap.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtfjuirsow.html

Py:   with lock: shared += 1
来源：http://hz.ivvv.top/gtiaimbnvw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tianlin.xyz/gtatfqjzua.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gthmduhihe.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtmqrkpjdf.html

Java: synchronized (this) { shared++; }
来源：http://hz.snrcjt.cn/gtpngfjusn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.birdmap.top/gtjqxtiykm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtpxqzcxew.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtpjhctzps.html

[O04] 定义异步函数并等待
来源：http://hz.xinyue.icu/gtmhleywew.html

Py:   async def f():⏎    await g()
来源：http://hz.gaohongyu789.top/gtadhyuboy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtfuijoflb.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtljfvbidb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hammf.cn/gttynkxreh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dashuyun.cn/gtvnxpmgit.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydjk.org.cn/gtjceiktki.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtdrvrthyg.html

C#:   async Task F() { await G(); }
来源：http://hz.smart0.xyz/gtcwxswjxc.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtwwdvuobx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtoygtkscg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtptejvohv.html

JS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtqhsvuycx.html

TS:   await Promise.all(tasks)
来源：http://hz.zhengqikj.top/gtoqxvvgxj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gtdamwssyj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtquhqfybw.html

Ruby: threads.map(&:join)
来源：http://hz.shzxlz.cn/gtgefsigtc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gtiywjvfkm.html

[O06] 使用进程池
来源：http://hz.c1oappe.top/gtxjeviwbn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtiiajnvvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtdyopyrni.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtopyzaseb.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtbewsoepm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuetiantiany.cn/gtkocikkss.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtzdilyxou.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gtnggumyww.html

C#:   Parallel.For
来源：http://hz.shanyushiyangtech.top/gtzclhaljh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqpppizez.html

P. 常用工具函数
来源：http://hz.jinqigufen.top/gtygveqsci.html

================================================================================
来源：http://hz.bjfxy.top/gtcgzrxgnv.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtwahrjxhx.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtopdtihgv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gtkaceribk.html

JS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtkfxappey.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtquuulaio.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtylqwypwi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigfzy.top/gtpxdruywc.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gtiincopie.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtqhieamcl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.bjfxy.top/gtcpfjpgpy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtwjgegmvt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxuanxn.top/gtubjnimvk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sxryk.cn/gtpuqyteox.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenlongwang.top/gtxonyfyvp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtsrxnaqrv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangtech.top/gtbxexjtas.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtajtmvnev.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtbwfmkact.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtzraawaon.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cashguo.top/gthfpowzui.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuanzx.com/gtxhzyzufd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtdslazspc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtvgxiudum.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtlylxytxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtrbbzhdsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gttwnmzpvj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtzmwzeirr.html

[P04] 求长度
来源：http://hz.fengsongda.top/gtilwwbgbs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gttwsabqov.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtqmlwpsry.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gttfxwzpzq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtszpgjeeu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj202588.top/gtehyntwyu.html

Go:   len(arr);  len(m)
来源：http://hz.yuanzhike.top/gtrywaczwb.html

Ruby: x.length;  x.size
来源：http://hz.hnxiangtu.top/gtaldscyok.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.mhx1999.top/gtsloyhxhw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gtizjoxmty.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtjymrgaff.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gtxwaizluy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.svipenyu.cn/gthcoyktdq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gthwzudzsa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtkxpyxmjt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtbssgaqab.html

Ruby: a == b
来源：http://hz.sweek.top/gtphwduaok.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtfnqehavw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hfpthk.cn/gtfhvpkmmo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cdnleiting.top/gtmisztbzu.html

PHP:  if (empty($x)) {}
来源：http://hz.guannengcc.top/gtmvvebuza.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhaomingkeji.xyz/gtjnbiioxq.html

TS:   if (x == null) {}
来源：http://hz.yueranfly.top/gtnmpkvzyg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cqqwz.cn/gttviydasd.html

Go:   if x == nil {}
来源：http://hz.jinghuilouyu.cn/gtppgclmov.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gogol.net.cn/gteivucuup.html

C#:   if (x is null) {}
来源：http://hz.mhx1999.top/gtlssevrdw.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtssgfwleo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gthwkaopld.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtxvkucbfo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtywwdhfeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtdewmulta.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gteaussfxw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgufenzy.top/gtxduslwvr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtnkgjjext.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtqueigdqw.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtgyoztktu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhongyouzk.top/gtnheszaya.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangdashe.top/gtfwjwwyfs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtzfsuhdca.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yangfankeji.com/gtilbcsrsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yanxiufei.cn/gtuhbkygwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ywan-chungtsiang.top/gtbbtuchpv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydzc1.top/gtwfkmxkan.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gogol.net.cn/gtropqvphg.html

================================================================================
来源：http://hz.sufxvd.cn/gtyyvyxfjb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtclrbducn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtstboezet.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtcuojzfyc.html

CREATE TABLE users (
来源：http://hz.cqqwz.cn/gtkkqfwoii.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtawfgwlpc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yueranfly.top/gtkxmwzktb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtcijjrqci.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtknogcsvf.html

);
来源：http://hz.sxryk.cn/gtfwatfamo.html

[Q02] 创建带外键的表
来源：http://hz.nanxinkj.top/gtfjvtnjyn.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gtnunnphpy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtiwnvpzxp.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gtolhssehk.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gthshuuvsj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ivvv.top/gtkbgrqkhp.html

);
来源：http://hz.mhx1999.top/gtoxhlipmy.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gtmnsenlxq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtnrdozgux.html

[Q04] 修改列类型
来源：http://hz.shuidangran.top/gtigyaista.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtrmpppqqf.html

[Q05] 重命名列
来源：http://hz.quarkkingdee.top/gtomndhdpx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ivvv.top/gtzeilhxhy.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gtikirwoxt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gtxexemymz.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtwlnbuibv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtublyoluo.html

[Q08] 创建普通索引
来源：http://hz.316326.xyz/gtiqiugkzz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtdfswvcbo.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtljiqljap.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtyiyfpwha.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtwsjmmsju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ywan-chungtsiang.top/gtvptcallh.html

[Q11] 一次插入多行
来源：http://hz.xuetiantiany.cn/gtvkjygisv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtqqupfqly.html

[Q12] 插入后取自增 ID
来源：http://hz.fzhhl.top/gtstxgwwjv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtaxrmeach.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtorpecbnw.html

[Q13] 忽略重复插入
来源：http://hz.ydzc1.top/gtlituqrwq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenzaomai.com/gttepogafo.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtajairxgk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shzxlz.cn/gtugdassyz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtrjntnsyt.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtkucwjcah.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gthwnkefop.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gthlwxnsoa.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtpdxmdamv.html

[Q17] 条件查询
来源：http://hz.redwolf501.top/gtmrutqwmg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtroxpcxxg.html

[Q18] 模糊匹配
来源：http://hz.nwbrower.top/gtynpuiklh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydjk.org.cn/gtonbiquot.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtkqpcchzm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtaxmyedjy.html

[Q20] IN 列表
来源：http://hz.pycfn.com/gtpjfuckkj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangdashe.top/gtkjlsurer.html

[Q21] 空值判断
来源：http://hz.9152youxi.cn/gtiantqmsp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtbbmrfjgv.html

[Q22] 排序
来源：http://hz.hammf.cn/gtvgzscewb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenjidiqi.icu/gtijekzvvq.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtntwsshmu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xinyue.icu/gtygokjugg.html

[Q24] 去重
来源：http://hz.jqgufenzy.top/gtqgwoeatl.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtbtgieuyw.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtetkfetwd.html


<!-- 参考信息 -->