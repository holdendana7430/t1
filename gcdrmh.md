代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtedldtpad.html

TS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gthvpsmieq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtpgdinycj.html

Go:   // 双指针从两端比较
来源：http://hz.ydjk.org.cn/gtxkhoqyos.html

Ruby: s == s.reverse
来源：http://hz.smart0.xyz/gtjwvzwxko.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.aizwys.cn/gtyqwxbpkr.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtaerbspvd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtzippdmij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fengsongda.top/gtxijzbuhq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yueranfly.top/gtpjegraaf.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtmpxoaesw.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtfsefrmsn.html

Go:   // 手写 map[int]int
来源：http://hz.aibaodan.cn/gtihvuythc.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtxopvpmsa.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.havefunace.top/gticsxhiwp.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtnicykqmq.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtfzuyixxh.html

PHP:  // 手写递归交换
来源：http://hz.cucudq.cn/gtsntgxcce.html

JS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtvhobkwmr.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtrqyumrgx.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gturrrirtz.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtvskqaetj.html

Ruby: arr.permutation.to_a
来源：http://hz.pycfn.com/gtciactatv.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtuvcrupoa.html

[N09] 栈与队列
来源：http://hz.xziqi.cn/gttgfqtyjw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.c1oappe.top/gtneojjzhf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtziticgxr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtqdpjosiy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gthssbwdto.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.9152youxi.cn/gtrqbytkuv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sweek.top/gtjpipkabe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ivvv.top/gttqpckyqw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhengqikj.top/gtdzmzqezn.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gtgxmgkopx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.feifeiyinyue.top/gtjbsrbtub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gtjtlausib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jiagoushi.top/gtwxlxvihm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtjrqppmbd.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigufen.top/gtgdpdumjl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gthdrwvkqz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtlnwhcrzf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daxiang520.top/gtzyvaxiel.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtvfdmvonm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtbtbkpcmo.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtrkegjzfo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtngvtkzte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtlxfipsvt.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtjqrtmdvf.html

Go:   // 手写递归
来源：http://hz.c1oappe.top/gthtlcdpun.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtjjaiuqrd.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtyenoehlu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.mhx1999.top/gtvyzebxrh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gtwbinirmv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtzeovoaiy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtqddwnhcc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtaleeajqr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtffyurxiz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guowangkeji.top/gtztujkjas.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gttoszvppz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtxperkjql.html

================================================================================
来源：http://hz.wangdashe.top/gtdelfghfn.html

O. 并发与异步
来源：http://hz.redwolf501.top/gtbsxbaerk.html

================================================================================
来源：http://hz.pycfn.com/gtrbhyklfr.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtzudcfcic.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgfzy.top/gteqmrejwa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtdkntshhn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhongyouzk.top/gtgapebzig.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtqxfzwejq.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtpwbvojal.html

Go:   go f()
来源：http://hz.vqdsnc.cn/gticruckqx.html

Ruby: Thread.new { f }
来源：http://hz.mhx1999.top/gttpgfcsda.html

C#:   Task.Run(() => F());
来源：http://hz.zhiwuduotai.top/gtiatadxtj.html

[O02] 使用线程池
来源：http://hz.gogol.net.cn/gthyhmnhqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydzc1.top/gtspmffxzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtnvbyzfba.html

JS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gteufzdlsb.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtpytwnfbj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtutvbngyp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gtncnazeem.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.kuanghao11.cn/gtmxbqlpix.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtbjtjvmaq.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigfzy.top/gtdidmpclf.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtecubwplp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sufxvd.cn/gtglvyqhaa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtoopablhu.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtgthgkuep.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtkihogncr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtpoystqax.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtlnffweuf.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtanjqgspa.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtgmqcempz.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtgvslzxdx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gtxbehprot.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtqmnnmell.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj202588.top/gtbgssfnaz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenzaomai.com/gtqrtubqij.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtmrzkwetq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gaohongyu789.top/gtjpjnxwtt.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtzesmyyws.html

[O05] 并发执行并等待全部完成
来源：http://hz.nwbrower.top/gtdiynvtrn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gtgiezmepg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtjstwaqxe.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtubdrhlra.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtxpomuoej.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cashguo.top/gtlrbcrzvh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtafskieiz.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtuepjzjgf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtpzutmjnz.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtlmppyune.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtcbqempmc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pengpengdd.cyou/gtwkumlwmk.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtqqmgggkg.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtpsibxade.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtryjhephy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtbihwomsv.html

Ruby: // fork 块
来源：http://hz.ehwqpu.com/gtmesejhzv.html

C#:   Parallel.For
来源：http://hz.birdmap.top/gttuiweflc.html

================================================================================
来源：http://hz.ivvv.top/gtjthssexx.html

P. 常用工具函数
来源：http://hz.smart0.xyz/gthcgyyuwg.html

================================================================================
来源：http://hz.ybcxt.top/gthpuhbhhj.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtrazxbkbl.html

Py:   str(uuid.uuid4())
来源：http://hz.0kj1m.cn/gtoowexdve.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuetiantiany.cn/gtrohrhydr.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gttrpvoytk.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtcbedggva.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtkfygairi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtemsulwya.html

Ruby: SecureRandom.uuid
来源：http://hz.yvedp.cn/gtykcmyjso.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ywan-chungtsiang.top/gtymtpbeyi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cqqwz.cn/gtmvzqnmyu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yangfankeji.com/gthiwbonyp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gzhubu.top/gtyaauyubu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtjodtiska.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtvuctsqfv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.c1oappe.top/gtlroluvih.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtbeetztaa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtspaauqon.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtkgkiaypg.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtpukjcbbx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtcbnwyuhj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yonumen.top/gtwnpfdapo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtauirbtke.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtygwkwgcr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dianchejie.cn/gtcvwlqvpg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ehwqpu.com/gtfmijitna.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtoyyofltx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangdashe.top/gtlirxzfdq.html

[P04] 求长度
来源：http://hz.smart0.xyz/gtxaidkuos.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtrisuopqo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtldwvdcyn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtixctwrdj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guowangkeji.top/gtdmhydlsn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhaomingkeji.xyz/gtiuutqnnp.html

Go:   len(arr);  len(m)
来源：http://hz.guowangkeji.top/gtygwciqmd.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtvrffwafz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258888.top/gtvxtrlepu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtrcadsido.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtnpbxcgad.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gaohongyu789.top/gtsgjbfxof.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sysykeji.top/gtetiuwyls.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtywfcqfxi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuanzx.com/gthyzrbbde.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtcporvzur.html

Ruby: a == b
来源：http://hz.gotoacloud.top/gtbgokakdu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtrgjdqeao.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258888.top/gtvdhjisxb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtefcrtsma.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtiyvaeqss.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtbopztyxt.html

TS:   if (x == null) {}
来源：http://hz.shuidangran.top/gtkvjwoepd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtwyccydlw.html

Go:   if x == nil {}
来源：http://hz.yj20258888.top/gtcnfddtmy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtilcmnvyp.html

C#:   if (x is null) {}
来源：http://hz.mhx1999.top/gtzctqyvgg.html

[P07] 防抖与节流
来源：http://hz.yvedp.cn/gtrctnbwyt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gthwqeozgz.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gtqemfqpqv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtbafffdmp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtdaimolyj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gtscrpldxa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtuunjgzrp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtyhcxnxbd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhoulong.xyz/gtvrqpckcc.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtcljcickr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhengqikj.top/gttnadhbuy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtcozggtur.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.aibaodan.cn/gtofdtnmov.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xylfe.cn/gthamzqlok.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pengpengdd.cyou/gtirfnaiev.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gzhubu.top/gtpjpdnblp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtuthcerwy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhongyouzk.top/gtssvjfchw.html

================================================================================
来源：http://hz.zycfv.cn/gtgqroxhrm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gtnzjizdcb.html

================================================================================
来源：http://hz.jqgfzy.top/gtnphpdztf.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtdgjwtqfu.html

CREATE TABLE users (
来源：http://hz.aizwys.cn/gtaxhoznqj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gttumnbyhc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgfzy.top/gtjssddwae.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gtgyfpillu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.52xcode.cn/gtrvohhsvm.html

);
来源：http://hz.wangdashe.top/gtzxcvcbbm.html

[Q02] 创建带外键的表
来源：http://hz.gogol.net.cn/gtzgdlrypu.html

CREATE TABLE orders (
来源：http://hz.snrcjt.cn/gtdzuypddx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtimbigqtg.html

user_id INT NOT NULL,
来源：http://hz.yueranfly.top/gtkyikvoqp.html

amount DECIMAL(10, 2),
来源：http://hz.jinyuanbaomall.cn/gtqzmlpipg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gotoacloud.top/gtlmtcfluc.html

);
来源：http://hz.tian-w.cn/gtapoxxhzg.html

[Q03] 增加列
来源：http://hz.yuxming.cn/gtnwcexquo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jyoumei.cn/gtobigavtt.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gttmycxdab.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jianghu66.top/gtpmguwlbl.html

[Q05] 重命名列
来源：http://hz.xuetiantiany.cn/gtxnkhvdch.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.vqdsnc.cn/gtaujgmacv.html

[Q06] 删除列
来源：http://hz.hammf.cn/gttohhkotg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jyoumei.cn/gtlxupoaln.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtrvugtufw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258888.top/gtqzodqnuj.html

[Q08] 创建普通索引
来源：http://hz.chenzaomai.com/gtowghfcqi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtsjgvshox.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtwhvhdezo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtehkwgbdx.html

[Q10] 插入单行
来源：http://hz.mhx1999.top/gtkdcmjwtd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gtdfuzvnoe.html

[Q11] 一次插入多行
来源：http://hz.meibo888.top/gtbidqxmad.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtjfnfvvxh.html

[Q12] 插入后取自增 ID
来源：http://hz.hywenlv.cn/gtxwangzde.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtkwekpabj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtlcftdpzw.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gtesrecojp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sysykeji.top/gtwwdwxwxs.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtbqfbuiqn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yangfankeji.com/gtzjljmiss.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtgxrbthno.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtzozjjbuf.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtlgrtfxfp.html

[Q16] 查询指定列
来源：http://hz.fzhhl.top/gtjfpawios.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtlrjyunwc.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gttmkvpood.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cheryme.top/gtkdclxlmw.html

[Q18] 模糊匹配
来源：http://hz.smart0.xyz/gtuljdxioo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtglajknpf.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtjmcerjxx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtkhfrixtq.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtgikdxhzk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtkrvhtlnc.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtdefvdjix.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenjidiqi.icu/gtzkabwwja.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtrwazrgcf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gthhrdsecm.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtbpenvchn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gthurwcuzc.html

[Q24] 去重
来源：http://hz.vqdsnc.cn/gttdgzmxmt.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gtzjfzvikg.html

[Q25] 只取前 N 条
来源：http://hz.jyoumei.cn/gtsauvgyhp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtovugqhfx.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtxfobrqrm.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhixingplan.top/gtwptesaqq.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gtwjvayilc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnxiangtu.top/gtqcfsalwn.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtvenyoiha.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtgdaxlgwm.html

[Q29] 最大最小值
来源：http://hz.ivvv.top/gtppiptqjk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtyusoaccs.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtbafsuwqo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtnlmgmtrw.html

[Q31] 分组后过滤
来源：http://hz.aizwys.cn/gtoatlblep.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtbmjjazjh.html

[Q32] 分组拼接字符串
来源：http://hz.zhoulong.xyz/gtbxqeputb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtgcxciaqm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jyoumei.cn/gtvbsgctpy.html

[Q33] 多列分组
来源：http://hz.xziqi.cn/gtycmzclnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.smart0.xyz/gtppiiupsu.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtneoacmaw.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtabqgrsnm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtgawgwnwq.html

) t WHERE rn = 1;
来源：http://hz.ydjk.org.cn/gtmdmwoynh.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtpdeagwgf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtwvzzdnul.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtazbjrxou.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtbxjrhwqs.html

[Q37] 右连接
来源：http://hz.xylfe.cn/gtzoesnmai.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ppjwa.cn/gtfyufaipa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daxiang520.top/gtyhjgfzre.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.quarkkingdee.top/gttcylofub.html

[Q39] 自连接（查上下级）
来源：http://hz.dianchejie.cn/gtntaprjir.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtftygvlqu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtndydctru.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gtglmvqrkq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtypsdniry.html

[Q41] 多表连接
来源：http://hz.hammf.cn/gtriykbzbb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sufxvd.cn/gtdejtucnx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tianlin.xyz/gtdayxaxys.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zdqjudy.top/gtqsyckggg.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtltbwhgpw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gtdxkkvuqj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.birdmap.top/gttdzacsrf.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtjaeoblyy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtybyvltnu.html


<!-- 参考信息 -->