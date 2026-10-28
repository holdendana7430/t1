代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtlhkegqib.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtwfpgnsgo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhaomingkeji.xyz/gtdxpfqhwd.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtqzkarrht.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtfrzdflra.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtaoidqvhj.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtdstsknpg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtgrxahgcx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fengsongda.top/gtkftshlxm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtpygbpumn.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtngwjuzkb.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtfnarvhjl.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gtgjayscbr.html

Ruby: // 手写 Hash
来源：http://hz.gotoacloud.top/gtwzmftlsv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pycfn.com/gtwcgljeai.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtsjhsqunr.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtwfgiivmm.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtgdzyiscy.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtymkedglc.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtmigxywcu.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtvaxzcnrr.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gthbpfdsfz.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gtqypvodrl.html

C#:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtgcqjvqpt.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtnkbocrvp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtvepdqngo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gticplekom.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtmndrvhte.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guannengcc.top/gtkgpgjtic.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtpbvrzqgc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtvfltenpx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gthujecqyy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.quarkkingdee.top/gtmdenuaty.html

[N10] 链表节点定义
来源：http://hz.zycfv.cn/gtqgghdvjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gtxjdjabby.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.quarkkingdee.top/gtzcrhyimt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtkfhlfudp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtjffvrxmt.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtolfwcpzj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtairwcofl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hfpthk.cn/gtryjjpfdd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtvqdhjitz.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gturzjbtdw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtjtpwehnz.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtaevvyqhd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtxkhqfzah.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtkjuwyyvi.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtblkegfrs.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtcxuwakuh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtezqgqedm.html

C#:   // 手写递归
来源：http://hz.zhijiandao.cn/gtskluecqj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigfzy.top/gtsbzzpqim.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hammf.cn/gtgjuomfjs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtdkxnukwl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtezyzguhi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtnahewdot.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtwxxdhilc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtgaznipze.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtladrsyec.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtnjlyqvkn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthirbhise.html

O. 并发与异步
来源：http://hz.ppjwa.cn/gtrbafdizf.html

================================================================================
来源：http://hz.sxryk.cn/gtisitdthv.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtpnvkvhqh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gteidbsyik.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtzlmneqcy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtklcvdjmu.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtbwguilaw.html

Java: new Thread(() -> f()).start()
来源：http://hz.fzhhl.top/gtlqunodks.html

Go:   go f()
来源：http://hz.ehwqpu.com/gtsskeecau.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtiabxoeih.html

C#:   Task.Run(() => F());
来源：http://hz.sweek.top/gtxyadxwvn.html

[O02] 使用线程池
来源：http://hz.sweek.top/gtzkmrknge.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.quarkkingdee.top/gtorjfcgkv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gthgtkqvae.html

JS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtmyqesnei.html

TS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtsmwpnrvw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtxrkvosay.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtgrlhnerd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtvuclpaib.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtuqyzwgwz.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtixlwzxpk.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gtcyjffkqh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hywenlv.cn/gtwndslqdp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhiwuduotai.top/gtbrgbrxff.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtwwtgicmv.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtqeplqzzl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydjk.org.cn/gtrbltwpsu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtoeodecmk.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtdjrshlue.html

[O04] 定义异步函数并等待
来源：http://hz.andypj.xyz/gthughgyib.html

Py:   async def f():⏎    await g()
来源：http://hz.wangdashe.top/gtsbxvcepo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinyuanbaomall.cn/gtqtwagiax.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtrmxzfjqn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shuidangran.top/gtfrpgjgfa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtprmxvokf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtbmcqzfzv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.kuanghao11.cn/gthtiiezir.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtcuraaczt.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigfzy.top/gtjnhflesn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtxdqcfdku.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtrtoiqkhy.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtxsmxqqbj.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtsedxxoaz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgfzy.top/gtrfnqexyh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtcwidnwvq.html

Ruby: threads.map(&:join)
来源：http://hz.zhengqikj.top/gtntyuncos.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sweek.top/gtcffjrqer.html

[O06] 使用进程池
来源：http://hz.52xcode.cn/gttpxbtctp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yvedp.cn/gtjdcvurhn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtnfcqzgyl.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gthxbyvcrd.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtwqjdklqj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtzugvsdxu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhongyouzk.top/gttkbxkyph.html

Ruby: // fork 块
来源：http://hz.guannengcc.top/gtqffgvefl.html

C#:   Parallel.For
来源：http://hz.yonumen.top/gtjxivurzt.html

================================================================================
来源：http://hz.yongpay.top/gthshgyxpx.html

P. 常用工具函数
来源：http://hz.hongshengwenyu.top/gtsejdtpwb.html

================================================================================
来源：http://hz.guowangkeji.top/gtxmdcpvnc.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtubhfrsck.html

Py:   str(uuid.uuid4())
来源：http://hz.hysaishi.cn/gtgdssuraw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtltkqefju.html

JS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtxmxmwoaw.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtqaidyddk.html

Java: UUID.randomUUID().toString()
来源：http://hz.yongpay.top/gtnzqweosf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guowangkeji.top/gttfmmvbjt.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtmdbgdcwj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yongpay.top/gtqwqfcfku.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pycfn.com/gtwrroefan.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtotfekdol.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtffdaurue.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtcitxnsmf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangtech.top/gtsugrewau.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtsdonnkzj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtdjpoctxo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtjejxkwcd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhengqikj.top/gtgywvtwuo.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gtmwjqsevr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtooqvgzuc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtfgjobsqt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtdhvjgftm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtuokvrqki.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtzykeccek.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gthxxgtuuq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtmrflppmm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.haohaochexian.top/gtfncfwujs.html

[P04] 求长度
来源：http://hz.cqqwz.cn/gtueecqqdw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtnergllyi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtkqkezdhy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtpgoxwkkg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtqmhqujzn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtgezhthkl.html

Go:   len(arr);  len(m)
来源：http://hz.ivvv.top/gteseuzxnw.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gtnhxpvzcl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gthlkcyumt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtxgqgfmai.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtmgwecque.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gtkkehknem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtwkahwadh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtdmlcwulp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nanxinkj.top/gtvfojritg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shangyingyoupin.top/gtryomiauf.html

Ruby: a == b
来源：http://hz.havefunace.top/gtuzmvqjtt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtflxcdeqm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtlcmmhndv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtxeeqepuc.html

PHP:  if (empty($x)) {}
来源：http://hz.guowangkeji.top/gtelwfavzo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gtfirkxvsc.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtjlpxoqfb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.52xcode.cn/gthbgtleev.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtagpejjxq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtbekgiave.html

C#:   if (x is null) {}
来源：http://hz.aizwys.cn/gthuairrxb.html

[P07] 防抖与节流
来源：http://hz.jqgufenzy.top/gtogrgbjny.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtjimsncyu.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gtpvcairdu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtjxualktv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtxlcyowvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fzhhl.top/gtbfcfzjgj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigufen.top/gteaxzavhe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gttoeuqfox.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.haohaochexian.top/gtppnrtakn.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtyhtsfbwh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgfzy.top/gtdomyjhtm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtvrgwptkr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gtrvgdiabp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxinkj.top/gtcnhuflbu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zdqjudy.top/gtgkdrqnqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.svipenyu.cn/gtzbdnklhl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.316326.xyz/gtfzkikoac.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtdxktfwik.html

================================================================================
来源：http://hz.haohaochexian.top/gtrqnzdbwq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtnmvowwsb.html

================================================================================
来源：http://hz.shuidangran.top/gtyxpwdfqi.html

[Q01] 创建表
来源：http://hz.chenlongwang.top/gtjjplgoev.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtxyefnfvu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtnxkquhwq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gturackkbn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.52xcode.cn/gttvbuyjnp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gtbhftdxpx.html

);
来源：http://hz.shanyushiyangkeji.top/gtkwplkolm.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtqykowxhu.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtgwydjmkf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtynfdbtgf.html

user_id INT NOT NULL,
来源：http://hz.iojbl.cn/gteuxspzqf.html

amount DECIMAL(10, 2),
来源：http://hz.chenlongwang.top/gtittrpxoe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigufen.top/gtlzolcpmn.html

);
来源：http://hz.xingfuxueyuan.xyz/gtjqmnklth.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtajffyqae.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtrjncngbx.html

[Q04] 修改列类型
来源：http://hz.zycfv.cn/gtkpmqqsob.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtrdgiruri.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtdrhjkaho.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258888.top/gtuhuhzckd.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtpiiqswty.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtxbuzlxth.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtmrtpmqhs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtcfpaawxi.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gttdwiiqdt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtsjugbhxv.html

[Q09] 创建唯一索引
来源：http://hz.jinqigufen.top/gtlaluojpw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yueranfly.top/gtxilubqwr.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtqzpiquzp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gtkzmkzmax.html

[Q11] 一次插入多行
来源：http://hz.haohaochexian.top/gtosvqzudg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtqaoogydo.html

[Q12] 插入后取自增 ID
来源：http://hz.cdnleiting.top/gtqyjrouti.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtmloqfuma.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtzwylfbbc.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtoatgimbk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtyhhnpydo.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtzmyhbhcx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yongpay.top/gtarhnxtzu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.kuanghao11.cn/gtonpgmfaz.html

[Q15] 查询全部
来源：http://hz.pycfn.com/gtnaggnqqi.html

SELECT * FROM users;
来源：http://hz.dianchejie.cn/gtlrgwtnjt.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtuqhteweg.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtiiejammb.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtyrtwhpki.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhiwuduotai.top/gthgbokgdz.html

[Q18] 模糊匹配
来源：http://hz.shzxlz.cn/gtrxfezyyv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigfzy.top/gtkbbymvid.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtqjiexhtq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gtdwtlezlq.html

[Q20] IN 列表
来源：http://hz.jqgufenzy.top/gthgxjlvka.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhengqikj.top/gtxmbxwxha.html

[Q21] 空值判断
来源：http://hz.jinyuanbaomall.cn/gtizpnehzh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtriejyyvu.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtzspwlnvh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gtyamepzyf.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtwriuxdvf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtlbwpvbiw.html

[Q24] 去重
来源：http://hz.ybcxt.top/gtsbmsluvc.html

SELECT DISTINCT city FROM users;
来源：http://hz.hammf.cn/gtiijoqrdu.html

[Q25] 只取前 N 条
来源：http://hz.jinyuanbaomall.cn/gtecmnfdjj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jlsjyb.cn/gtwgpmhkih.html

[Q26] 计数
来源：http://hz.daria6918.cn/gtxxmsbppn.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtdmqhdjnx.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtpudtmnyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtwijgahlz.html

[Q28] 求和与平均
来源：http://hz.jinyuanbaomall.cn/gtsemxpskg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jyoumei.cn/gtuwidfwma.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtczmmekpp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangshuangyany.cn/gthmzfoxmk.html

[Q30] 分组统计
来源：http://hz.redwolf501.top/gtgjvjpopa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtdzkczwbv.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtugxhttkg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtwrviwjgz.html

[Q32] 分组拼接字符串
来源：http://hz.quarkkingdee.top/gtaiebszwy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtcyytfkdh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.mhx1999.top/gtxskdsshj.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtogpgcxft.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtmdgnchqm.html

[Q34] 每组取第一条
来源：http://hz.chenjidiqi.icu/gtspowafvo.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtrgwkczrp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtkurcwmpf.html

) t WHERE rn = 1;
来源：http://hz.bjfxy.top/gtddntyotd.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtdavypmwz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtltvwyojk.html

[Q36] 左连接
来源：http://hz.hnqzz.top/gtfzyipgpf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtgbevlypy.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtupbiqdex.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtoxbcfczn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gteasglfvg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtprjvgpxo.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtlrladksk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtcnbsbqie.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gtvzfpgifn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtacijrbyg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenzaomai.com/gtkufegoex.html

[Q41] 多表连接
来源：http://hz.hnxiangtu.top/gtlsturmps.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxinkj.top/gtrfqkokdp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtcyzceyix.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ybcxt.top/gtknloxwbr.html

[Q42] 连接条件附加过滤
来源：http://hz.gotoacloud.top/gtbmcdthqs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtcxedsgtl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtzfxpqjto.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtbihpncne.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.vqdsnc.cn/gturnzmwnk.html


<!-- 参考信息 -->