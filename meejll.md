代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gtkeuhfbct.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gtvmrnwkss.html

Py:   s == s[::-1]
来源：http://hz.kuanghao11.cn/gtzpodfsrv.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gtamtipkbb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtscrvujsj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtyxijzfnc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtaddsaloe.html

Go:   // 双指针从两端比较
来源：http://hz.cqqwz.cn/gtcxtjgwvl.html

Ruby: s == s.reverse
来源：http://hz.yongpay.top/gtifcqbpjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtxkqwkckd.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtctsqiony.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtmrmivvtf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtyuydeddc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtwpdhykko.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtnmcitwst.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gthkdqnrvr.html

Go:   // 手写 map[int]int
来源：http://hz.hnxiangtu.top/gtqypkdqec.html

Ruby: // 手写 Hash
来源：http://hz.yongpay.top/gtlzzvryqx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuetiantiany.cn/gtkxipssrd.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtjexidiyw.html

Py:   itertools.permutations(arr)
来源：http://hz.zycfv.cn/gtgcjbladn.html

PHP:  // 手写递归交换
来源：http://hz.cheryme.top/gtldhkaqnk.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtngtllbfw.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtgatoyhlc.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtupvommgd.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtrivjgqqh.html

Ruby: arr.permutation.to_a
来源：http://hz.zdqjudy.top/gthneqmasf.html

C#:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtwgqlvcjj.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gtrbbtgktt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtmhwltsto.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtimcsotan.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtnslnhhqg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.iojbl.cn/gtxwbpberl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtkwyedkku.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenjidiqi.icu/gtymkhacwk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtqlhqsico.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jyoumei.cn/gtlorcummb.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtcxgzpily.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtyqmsqqcx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxinkj.top/gtxuuvlgds.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtuhoyxmkm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtpnxgokrq.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gthwqtsqgz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtgaqwagqb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gtctjctkkd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xinyue.icu/gtuyfkcrkf.html

[N11] 二叉树中序遍历
来源：http://hz.yj202588.top/gtmuphybwt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtnfwssttu.html

PHP:  // 手写递归函数
来源：http://hz.0kj1m.cn/gtuvtoybfm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gttidfwrft.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtiidftqpc.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtrygffsny.html

Go:   // 手写递归
来源：http://hz.iojbl.cn/gtecapemvr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtptasbokj.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtykyvwftl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigufen.top/gtkrwmqvue.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yongpay.top/gtcufckqgu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shuidangran.top/gtwcmpxrxg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtmfklzsbd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtejkwrnxq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtybkeiewb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gtaljmmixe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hfpthk.cn/gtsubvekey.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gthkxymdtq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtghbokwhg.html

O. 并发与异步
来源：http://hz.xingfuxueyuan.xyz/gtaqjgceca.html

================================================================================
来源：http://hz.cheryme.top/gtfhgfzpac.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtlzpxfvet.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dashuyun.cn/gtcmvaevlp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtfeygnuzc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yangfankeji.com/gtrippvrla.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtvwetyojw.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtgyoolwet.html

Go:   go f()
来源：http://hz.chenjidiqi.icu/gtepfkjwur.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gticfjxmum.html

C#:   Task.Run(() => F());
来源：http://hz.wangdashe.top/gtldldplhh.html

[O02] 使用线程池
来源：http://hz.yj20258888.top/gtdtiiwqpm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtniigonld.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtqseliutb.html

JS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtsmzfgdsu.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtmqdaqwhh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.quarkkingdee.top/gtoguouhfz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.vqdsnc.cn/gtzhcvohdh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtznszmmni.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gthlfnktyo.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gttdqkdmhg.html

Py:   with lock: shared += 1
来源：http://hz.nanxinkj.top/gtafyhwrge.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtjhxpzuwd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxinkj.top/gtpfdmxerd.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtgtgxcjky.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gtwpsncrni.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigufen.top/gttgtfsqxo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.feifeiyinyue.top/gtddsyheqq.html

C#:   lock (gate) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtddvhqpkh.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gtivmsdagg.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtbmmxefif.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jiagoushi.top/gtiquqvfgj.html

JS:   async function f() { await g(); }
来源：http://hz.gzhubu.top/gtxgcrgulv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtxywqzfer.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.kuanghao11.cn/gtctoesqqa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhongyouzk.top/gthihfazhs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtpdvmqamx.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gthunlgzvw.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtuuszelfj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtbywhirya.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pycfn.com/gtkokuvhrx.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtrmrggpiy.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtlvtftqih.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.52xcode.cn/gthhqdveuu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yueranfly.top/gtzkjeuxyb.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtqcjbbnon.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gtsulvojti.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtmjsaoxbu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydzc1.top/gtbnrflvgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhaomingkeji.xyz/gtoajotiev.html

JS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtlhpcndgy.html

TS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtskbaaykc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.iojbl.cn/gtujdbllvf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.redwolf501.top/gtjddcnhee.html

Ruby: // fork 块
来源：http://hz.gogol.net.cn/gtsyfziqnr.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtofgezlng.html

================================================================================
来源：http://hz.sxryk.cn/gtblyjypst.html

P. 常用工具函数
来源：http://hz.dashuyun.cn/gtdmvrumsd.html

================================================================================
来源：http://hz.smart0.xyz/gtyiyfmakd.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gtdywvpxyk.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtngwfurlc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gtvtucmokz.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtkeekixmz.html

TS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtglvmjazt.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtjmurlkyz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtirtyfqwl.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258.top/gtavvleujs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtpvnedxry.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtdcnjbhta.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pengpengdd.cyou/gtxstfpsqt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtldnlwahz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ivvv.top/gthmsxvglv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtsblgvsba.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nwbrower.top/gtoiegsziv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gthszmjpxx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtpfnhoylh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtbhtbauhv.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtzsupbxhi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtscyqdruy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxinkj.top/gtvwvrrpoz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtufzmkumh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtzayydirt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtqlclbsjk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gtuuyrjfos.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hywenlv.cn/gtvejrmqgx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtuswrtrgw.html

[P04] 求长度
来源：http://hz.316326.xyz/gtygqligwk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gzhubu.top/gtmnioldfo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtzxastjeb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtwgagrbub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtvjzniqko.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtlawbkwxe.html

Go:   len(arr);  len(m)
来源：http://hz.jiagoushi.top/gtpptajacm.html

Ruby: x.length;  x.size
来源：http://hz.havefunace.top/gtokjndydz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtdiyyjsyt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.9152youxi.cn/gttiavvczl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jiagoushi.top/gtxryybhhi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangdashe.top/gtuezghfzt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtfkhbstvz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtjosuommc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtkowgtdpd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydzc1.top/gtvipisgom.html

Ruby: a == b
来源：http://hz.nwbrower.top/gtdijuflbr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtujvjisfm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jlsjyb.cn/gtomhucuoh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhixingplan.top/gtexyjaqvb.html

PHP:  if (empty($x)) {}
来源：http://hz.tian-w.cn/gtndsuozpo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgfzy.top/gtniiekmhc.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gtcojpckig.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.haohaochexian.top/gteedbjjrs.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtevhiuner.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtumpolyfg.html

C#:   if (x is null) {}
来源：http://hz.yj202588.top/gtxnupubtp.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtadunoqur.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.meibo888.top/gtngmyxwop.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtvlsuoikt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtmsgmlxdx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtmugncvky.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hysaishi.cn/gtxhqqgdtp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daxiang520.top/gtoreauocj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hywenlv.cn/gtsszainpt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtvjcljoyf.html

[P08] 处理浮点精度问题
来源：http://hz.yanxiufei.cn/gtvbexnnce.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuetiantiany.cn/gtbphvlgpf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtyavihchp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gtrgpnxuqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtsagiswlm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sufxvd.cn/gtgnkylqsx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cucudq.cn/gtapktvwhf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtiyreholz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.mhx1999.top/gtfxwghgdu.html

================================================================================
来源：http://hz.daria6918.cn/gtsnlzibqv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gtlcehmuml.html

================================================================================
来源：http://hz.haohaochexian.top/gtobbndnuv.html

[Q01] 创建表
来源：http://hz.zycfv.cn/gtwhscihtl.html

CREATE TABLE users (
来源：http://hz.ehwqpu.com/gtiuetmfnx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gtafhlkanu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.9152youxi.cn/gtgwpeigiu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gttwnnknab.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gtqzyvfmto.html

);
来源：http://hz.aibaodan.cn/gtfpvhocjs.html

[Q02] 创建带外键的表
来源：http://hz.ybcxt.top/gtmagihxgz.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtrdnuzgvn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtpgrmrriz.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtivaqsbyi.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gthazmbeqz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gthglrotqc.html

);
来源：http://hz.jqgfzy.top/gtjtbtxlmn.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtacsgcdwf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtdlvtdxiz.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gtxzsagweq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtarfcuqkm.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtpgojihwh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtodnsyiig.html

[Q06] 删除列
来源：http://hz.zhixingplan.top/gtwgyjlome.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenzaomai.com/gtryxavjze.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtgjgstdaj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtvgylwrjb.html

[Q08] 创建普通索引
来源：http://hz.tanke756.top/gtkflbahwx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtzdlxicxc.html

[Q09] 创建唯一索引
来源：http://hz.ppjwa.cn/gtemyvzcgm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtshftuezj.html

[Q10] 插入单行
来源：http://hz.c1oappe.top/gtiknmdqdq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtftqlcblr.html

[Q11] 一次插入多行
来源：http://hz.tanke756.top/gtyxdgzuge.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cucudq.cn/gtrpjdildb.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgufenzy.top/gtlwxzxzbo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydjk.org.cn/gteemfwlox.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtspnmzjxs.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtvjvidyvn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.feifeiyinyue.top/gtuxjidczv.html

[Q14] 存在则更新（upsert）
来源：http://hz.jlsjyb.cn/gtbymeioyk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jianghu66.top/gtucxwvtyh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gotoacloud.top/gtibnuyoyg.html

[Q15] 查询全部
来源：http://hz.chenjidiqi.icu/gtynukkcqa.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gteolceqxt.html

[Q16] 查询指定列
来源：http://hz.jlsjyb.cn/gtktwczlym.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtnpmquffb.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtmagkcpjg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gogol.net.cn/gtptjkquww.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtfolhuwmm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gttnnelwze.html

[Q19] 范围查询
来源：http://hz.daxiang520.top/gtdatfjepq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jlsjyb.cn/gtxbqlvisc.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtsleefxpv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtcztksryr.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtqjhekqbj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnqzz.top/gthwuxhkpa.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtsmbfebzf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cqqwz.cn/gtwqtrcjrw.html

[Q23] 分页
来源：http://hz.xuetiantiany.cn/gtdyhfmslm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.meibo888.top/gtfqroqqku.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtmwfspmcz.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtebvfjzus.html

[Q25] 只取前 N 条
来源：http://hz.hnxiangtu.top/gtehbjjqan.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtvabfkllq.html

[Q26] 计数
来源：http://hz.cashguo.top/gthyczsktn.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxinkj.top/gtkgcksltc.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtsuzxxjes.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xylfe.cn/gtrndrjypx.html

[Q28] 求和与平均
来源：http://hz.hongshengwenyu.top/gtedjxiqso.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cdnleiting.top/gtkfutfolm.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtjsjwyejq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bjfxy.top/gtlbozxvuf.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtmhblpczm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtkrpirkqh.html

[Q31] 分组后过滤
来源：http://hz.hongshengwenyu.top/gtzidxazht.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cashguo.top/gtqdlimpfn.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtbetitbaf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtteiejxcz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhixingplan.top/gtmkjvrhqw.html

[Q33] 多列分组
来源：http://hz.aizwys.cn/gttfeyodbh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtpdwmwqpt.html

[Q34] 每组取第一条
来源：http://hz.birdmap.top/gtqylptpnz.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gtwwqlplyu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtvbwktboa.html

) t WHERE rn = 1;
来源：http://hz.hnqzz.top/gtkvvwzpzp.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtmtjnuwua.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtqamkbdiv.html

[Q36] 左连接
来源：http://hz.yuxming.cn/gtcqogtrom.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtbrpwapxy.html

[Q37] 右连接
来源：http://hz.havefunace.top/gtlrqhsbnb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtjkksucjj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gtvyuwcgnr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cashguo.top/gtkhnkrass.html

[Q39] 自连接（查上下级）
来源：http://hz.ybcxt.top/gtplrzjjib.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtzkpvfemd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtzhoqxvaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sxryk.cn/gtlfzqcxuz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xziqi.cn/gtpjlaeebm.html

[Q41] 多表连接
来源：http://hz.jyoumei.cn/gtzpooklyi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigufen.top/gtswvsieyr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtduyjxhxg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xinyue.icu/gtzcxizbek.html

[Q42] 连接条件附加过滤
来源：http://hz.sxryk.cn/gtosykhpox.html


<!-- 参考信息 -->