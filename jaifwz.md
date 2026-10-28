代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtgrhdrcxn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtnpwxvwzt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangdashe.top/gtsfdaednu.html

Ruby: a.gcd(b)
来源：http://hz.mhx1999.top/gtfpamrwla.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtvcmywnrl.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gttzonsicw.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtkgdfayqy.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtexqwvrqn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtbhtqnvnr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtqdgcjfai.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtkkelidwl.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtwwmwiovs.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtruvocmyg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtqpqcssdl.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtbzagvanf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daxiang520.top/gtzykxjmlp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtuobwzgee.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yangfankeji.com/gtthtilpyz.html

TS:   // 手写 Map<string, number>
来源：http://hz.vqdsnc.cn/gtcaupqepf.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtrprxlefj.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtrxieuidk.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtfqestudt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gtgtafshzv.html

[N08] 生成全排列
来源：http://hz.feifeiyinyue.top/gtmukxbsna.html

Py:   itertools.permutations(arr)
来源：http://hz.andypj.xyz/gtqjfvyfud.html

PHP:  // 手写递归交换
来源：http://hz.dianchejie.cn/gtshdyorei.html

JS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtyjxnuwpz.html

TS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtxdoogepj.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtwilxtarc.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gtityjczpi.html

Ruby: arr.permutation.to_a
来源：http://hz.ivvv.top/gtjyvafowi.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gthxtffujs.html

[N09] 栈与队列
来源：http://hz.aizwys.cn/gtaoqqeypu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtxvsutvmr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtsbhruovl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gtzhwqyosb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pengpengdd.cyou/gtbjoatmlx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.kuanghao11.cn/gtxlzopchs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtksqlumnb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtjjsixibm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.snrcjt.cn/gtjarqsysp.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangtech.top/gtykhcvywn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtreztvsao.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gtngqeogzx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pengpengdd.cyou/gtwwavjrlv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinghuilouyu.cn/gttyirszww.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gthtumlisn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gtxptjesad.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhaomingkeji.xyz/gtdklnrcui.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtsnidppyi.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangtech.top/gtigaxboiv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtfjhejskl.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtyroehvry.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtrgbadvtd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtyazhsnyr.html

Java: // 手写递归
来源：http://hz.wangdashe.top/gtthdtwnqt.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtvbtxcqta.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtnakavxhq.html

C#:   // 手写递归
来源：http://hz.zycfv.cn/gttyjrdfrk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gthmwpmlps.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gttppsgrnn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gtyqzzdyok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtfnpspoxa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtjycssndt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtffknexgz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gtdwnaiszj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yonumen.top/gthzzmusbp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtxeetgbnm.html

================================================================================
来源：http://hz.0kj1m.cn/gtaimrkxcu.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtqprmenji.html

================================================================================
来源：http://hz.tanke756.top/gtswqqaftq.html

[O01] 启动一个线程
来源：http://hz.jqgfzy.top/gtkgakzwic.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gtuczhruyz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.andypj.xyz/gtgylhywmn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gttbjinmpy.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtoonlpyfh.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtrriieuyh.html

Go:   go f()
来源：http://hz.tian-w.cn/gtsufostnr.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtsfqerhxz.html

C#:   Task.Run(() => F());
来源：http://hz.yuxming.cn/gtebayqyqv.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gtwespuvaj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gotoacloud.top/gtqznqzsjz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtiyxpcspr.html

JS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtpcewqmiq.html

TS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtjsacgsvc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtbnordxau.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gttxfvausj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.0kj1m.cn/gtelsvurch.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtescvgjze.html

[O03] 加锁保护共享数据
来源：http://hz.ydjk.org.cn/gtnaatqvmj.html

Py:   with lock: shared += 1
来源：http://hz.wangshuangyany.cn/gtwcopfxuc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtdqygnlsk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gtbenbaamp.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtdijraudj.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhiwuduotai.top/gtfzappcss.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gttcrgojds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yanxiufei.cn/gtxdmtybjz.html

C#:   lock (gate) { shared++; }
来源：http://hz.9152youxi.cn/gtnypatmaz.html

[O04] 定义异步函数并等待
来源：http://hz.pycfn.com/gteibqtxfv.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gtyfpuqcxe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtjwikjztu.html

JS:   async function f() { await g(); }
来源：http://hz.316326.xyz/gtiqfasido.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gthraazkzb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cheryme.top/gtvxhehulr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj202588.top/gtmgktjfqu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.mhx1999.top/gtmvsylmyv.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtgwmgufrb.html

[O05] 并发执行并等待全部完成
来源：http://hz.jlsjyb.cn/gtietxtpba.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtubtsujyn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangkeji.top/gtpynwgrqu.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtiqcgvykt.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtsdawajno.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xingfuxueyuan.xyz/gtccrmbrnx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gtsuhungro.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtvfvmvpnu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cqqwz.cn/gtrcigailh.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtuqdqqpwq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yangfankeji.com/gtfokuufcq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guannengcc.top/gthqvmaigr.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtiatqmtqu.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtlwzkyjgb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gthhiggotm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.redwolf501.top/gtjrqqhpiv.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtvgaxnjzf.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gttjdcagbd.html

================================================================================
来源：http://hz.hammf.cn/gtuwxfbbfl.html

P. 常用工具函数
来源：http://hz.hnxiangtu.top/gtlcarfetc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpuqqtrva.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gtojmcvtjx.html

Py:   str(uuid.uuid4())
来源：http://hz.hywenlv.cn/gtbyrzltoa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhongyouzk.top/gtszdiimtn.html

JS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtlvkhwyri.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtlndbkdwi.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtzsiywkdk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtkluglrwr.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gtylgaaavi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yonumen.top/gtsaerzgjs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtagxtlybn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtzmudmhhm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sweek.top/gtxdopicaz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ywan-chungtsiang.top/gtvgwpfpgk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtwaebxdbd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtoargbcmp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtpjyylmtu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtdprpucym.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxinkj.top/gtxsfqylie.html

[P03] 生成短随机字符串
来源：http://hz.316326.xyz/gtwpfhiieg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aizwys.cn/gteyxkubeh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.c1oappe.top/gtmfacmclv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtnywgicvu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtnjlthged.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtassswfec.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtdekuktik.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhixingplan.top/gtmfusuupk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jianghu66.top/gtkhnamkij.html

[P04] 求长度
来源：http://hz.52xcode.cn/gtklarrbgx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigfzy.top/gtxuxawium.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gttstgqviw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtavrentty.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gthgxmabvs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtaakbqscz.html

Go:   len(arr);  len(m)
来源：http://hz.fengsongda.top/gtpjbgnarm.html

Ruby: x.length;  x.size
来源：http://hz.yvedp.cn/gtzmuanwlk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtcfflrqjh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shangyingyoupin.top/gtbcvkdrwv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtmcbbwlxb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhongyouzk.top/gtykkufhst.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.quarkkingdee.top/gtlzppdceq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnxiangtu.top/gtvixzivof.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtdranjvcy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xziqi.cn/gtxyomyfwh.html

Ruby: a == b
来源：http://hz.hfpthk.cn/gtmsbiobpx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhiwuduotai.top/gtjbqouhii.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtgxnbrjja.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxuanxn.top/gtlygkjnnw.html

PHP:  if (empty($x)) {}
来源：http://hz.mhx1999.top/gtygxfxblo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtpvpiipez.html

TS:   if (x == null) {}
来源：http://hz.yueranfly.top/gtwidxnirj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtmkscqtun.html

Go:   if x == nil {}
来源：http://hz.zhaomingkeji.xyz/gtyzymltay.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtstldganh.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gtqgkgdkkq.html

[P07] 防抖与节流
来源：http://hz.nanxinkj.top/gtwsbwobow.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtjjtqaesr.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtvrhpzulv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtjfoztuwi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtzvictzve.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yongpay.top/gtwlkucxmp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtglrqxssc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.haohaochexian.top/gtjpqbkwlb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtuvncencf.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtuwtnwubr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhoulong.xyz/gtzengrcqk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangkeji.top/gtomhnrofq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gtzcdvyhge.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtcgwfsqsf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenlongwang.top/gtlekehugw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydjk.org.cn/gtsoopxpqt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtfxxaembh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yanxiufei.cn/gtbssqcrsw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbefkkgan.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtrnoznwqk.html

================================================================================
来源：http://hz.jianghu66.top/gtmtkelsaa.html

[Q01] 创建表
来源：http://hz.sweek.top/gthwlswanr.html

CREATE TABLE users (
来源：http://hz.zhengqikj.top/gtvwaeoqjj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gthtrkgoea.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pengpengdd.cyou/gtjqzfstli.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nanxuanxn.top/gtkedturps.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ywan-chungtsiang.top/gthbdutypy.html

);
来源：http://hz.jlsjyb.cn/gtotikwurl.html

[Q02] 创建带外键的表
来源：http://hz.pycfn.com/gtvwfvjtuo.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtpyxtnzbd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtoxowkkvz.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtqtyzydlg.html

amount DECIMAL(10, 2),
来源：http://hz.zdqjudy.top/gtobtoacad.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhijiandao.cn/gtyzcyizhn.html

);
来源：http://hz.zycfv.cn/gtnwcliffq.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtduetkawn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhaomingkeji.xyz/gtefoxnats.html

[Q04] 修改列类型
来源：http://hz.pengpengdd.cyou/gtizlekmzj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zycfv.cn/gtadunpuvs.html

[Q05] 重命名列
来源：http://hz.guowangkeji.top/gtlmqclnng.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gteeoatuhs.html

[Q06] 删除列
来源：http://hz.chenzaomai.com/gtsqlpgmyb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtyiodkglh.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtqsrpweoq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gteeclgzri.html

[Q08] 创建普通索引
来源：http://hz.cucudq.cn/gtfthkbhsc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jianghu66.top/gtdbyxvnbk.html

[Q09] 创建唯一索引
来源：http://hz.cucudq.cn/gtwmcagxrv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtsecruxki.html

[Q10] 插入单行
来源：http://hz.zhoulong.xyz/gtezwahfpj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xingfuxueyuan.xyz/gteakykblo.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtdmpuokgu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cdnleiting.top/gtaskoeubf.html

[Q12] 插入后取自增 ID
来源：http://hz.aizwys.cn/gtnzklujos.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtzlzcgcix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258888.top/gtqilviuxb.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtpacjbsqy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtmrocxfom.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gtfcbtswfo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sweek.top/gtcyafqdkv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gthchnesxj.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gtbyjvnlif.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gtagqagfll.html

[Q16] 查询指定列
来源：http://hz.tianlin.xyz/gttpajwdti.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtnhludtyk.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtohlhzfpb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtcrqjbtqv.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gtbbczrbyh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtyggrsgso.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtoxwsetfg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jianghu66.top/gtpjfpacsx.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtyolofbyz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cqqwz.cn/gtflhhvwei.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtqobwguzt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtwdmwcfmu.html

[Q22] 排序
来源：http://hz.cashguo.top/gtxhydtqpj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gtpdwjbcwc.html

[Q23] 分页
来源：http://hz.guannengcc.top/gtsnqpgtls.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhixingplan.top/gtktgvvlat.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gtsiovdkrb.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gtevcdqzfp.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtohospveu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtpurbxkdv.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtomppnlgf.html

SELECT COUNT(*) FROM users;
来源：http://hz.guannengcc.top/gtyhgnpqyd.html

[Q27] 条件计数
来源：http://hz.ehwqpu.com/gtreotssjp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gtqcdoouar.html

[Q28] 求和与平均
来源：http://hz.yongpay.top/gtliywvezg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gtmibdbakz.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gtuyxezhta.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sysykeji.top/gtbgwcyljc.html

[Q30] 分组统计
来源：http://hz.gogol.net.cn/gtshsqsuda.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtnzxvbmmy.html

[Q31] 分组后过滤
来源：http://hz.xylfe.cn/gtpjgsjefv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtyabqgxhl.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtfdwmarga.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gttoljrajy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yonumen.top/gtbttklblb.html

[Q33] 多列分组
来源：http://hz.zycfv.cn/gthyqmuexu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xylfe.cn/gthbvraldo.html

[Q34] 每组取第一条
来源：http://hz.yvedp.cn/gthphscxsw.html

SELECT * FROM (
来源：http://hz.yangfankeji.com/gtiopjduoo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtbiqykzes.html

) t WHERE rn = 1;
来源：http://hz.ivvv.top/gtwqqjgxmp.html

[Q35] 内连接
来源：http://hz.316326.xyz/gtmtcujgko.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtsqhmbnac.html

[Q36] 左连接
来源：http://hz.xingfuxueyuan.xyz/gthsiwabcm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtmtntlaps.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gtbhlbkbgo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258888.top/gtiilpcofn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtyliuoooa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtaxufvmjl.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtmxfipswq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gttecgpwxc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtmkremffp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtghgupbnd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pycfn.com/gtszknbrpi.html

[Q41] 多表连接
来源：http://hz.hammf.cn/gtdzrxnipu.html


<!-- 参考信息 -->