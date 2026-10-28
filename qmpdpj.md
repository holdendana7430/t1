代发 wailian999

[N05] 最大公约数
来源：http://hz.hongshengwenyu.top/gtevizjqco.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gtwnhooxhn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtfyirxkgm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtdhonwdbz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtbcvuxawo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtoaosjpqu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yvedp.cn/gtqudvwzui.html

Ruby: a.gcd(b)
来源：http://hz.hnxiangtu.top/gtchnurriz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gtemzdqsqb.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtxtrmynbj.html

Py:   s == s[::-1]
来源：http://hz.0kj1m.cn/gtmjjjifej.html

PHP:  $s === strrev($s);
来源：http://hz.316326.xyz/gthlcbszbx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtzggcclkc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtqhkxwmsw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gttzvkqngr.html

Go:   // 双指针从两端比较
来源：http://hz.aibaodan.cn/gtgptecnin.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtodkbaoil.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtvdclaodb.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtofkrqfqy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhoulong.xyz/gtziglonns.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtlvimkdtn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtrauhhvag.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtztbmaaui.html

Java: // 手写 HashMap
来源：http://hz.jiagoushi.top/gtwmacxrsb.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtsuqmyxps.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gtawuwesxy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtelwtxmgv.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gtvrzlspfv.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtyxhuqfbe.html

PHP:  // 手写递归交换
来源：http://hz.pycfn.com/gtpuokdfur.html

JS:   // 手写回溯递归
来源：http://hz.sweek.top/gtnuqkgyvm.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtttwsrsuu.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtagfhsyvb.html

Go:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtdvovbqfh.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtnbcywibx.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtsxmnecpz.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtnmpxzhfb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhengqikj.top/gtiuoearvc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zdqjudy.top/gtowipvylp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtladzhnnm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tian-w.cn/gtwcuvehgn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtbkqbuqpj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtjjzjnsqx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtosjqvuvf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtlwhzfibv.html

[N10] 链表节点定义
来源：http://hz.cucudq.cn/gtktqgwbzb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtmbpgpnho.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtqrqeqtdy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xingfuxueyuan.xyz/gtquuujsuc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigfzy.top/gtxalmhvzl.html

Java: class Node { int v; Node next; }
来源：http://hz.jinghuilouyu.cn/gtplelxxvj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtsqkmwprz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gtktayslyt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.vqdsnc.cn/gttoqmixxp.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtgdsdgfpc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtxxjhtaap.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtnnbtqpgc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtehwffzze.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtphokejjr.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtxhhbkhdc.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtabflqupb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ybcxt.top/gtyvgwqxzw.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtynodfmvd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gotoacloud.top/gtlpblncvl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.meibo888.top/gtapqyndxy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daxiang520.top/gtaprivgoj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtxnxefeak.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtmkniauuk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtrrzueqzh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtyqiyetgj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gtviptyujp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtaygeinst.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmzslpoxm.html

O. 并发与异步
来源：http://hz.cdnleiting.top/gtgbbexzwz.html

================================================================================
来源：http://hz.yj20258.top/gtxmftogox.html

[O01] 启动一个线程
来源：http://hz.hnqzz.top/gtqwhrzuvb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtnqmaaaiv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnqzz.top/gtpvmmfeku.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtymqfzfho.html

TS:   // 同 JS
来源：http://hz.nanxuanxn.top/gtqwvsmxmu.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtqbamobrz.html

Go:   go f()
来源：http://hz.9152youxi.cn/gtknkeqelg.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gtjloyafze.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangtech.top/gtvckcfavs.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gtswpspehn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtslynjuho.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtfnmnqulf.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtibwxzicp.html

TS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtieonydsf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gttqrkubvc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenzaomai.com/gtsywglkqn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtoytpnjgu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtrvbbbnuc.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtzghmiltr.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtfsgbkxvr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenjidiqi.icu/gtjlcipmag.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ehwqpu.com/gtcaaorgde.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtkotnfkkv.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gtnkxbrtqa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhaomingkeji.xyz/gtzwtvmcnp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtemqasems.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtxhonbjea.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtsdngbkpn.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtbfpkxrtp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtafaeebta.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtmeqimmmh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtpbacuotk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtnwdnibfu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtfjphnljl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtucvzdeus.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtuwzrlkon.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtjxbclxad.html

Py:   asyncio.gather(*tasks)
来源：http://hz.vqdsnc.cn/gtwanyaopt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.birdmap.top/gtlzlmwfgd.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtlqkzvrpd.html

TS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtqzrnlnhv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtwovphxag.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shangyingyoupin.top/gtepjvilnf.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtvyhjzzoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtnaldieoz.html

[O06] 使用进程池
来源：http://hz.wangdashe.top/gtggcgawhl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtmvacdhnk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jyoumei.cn/gtqwazoptu.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtclatuayf.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtzhnrvfem.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xziqi.cn/gtgmqjjkxj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinyuanbaomall.cn/gtsnfnslvz.html

Ruby: // fork 块
来源：http://hz.guowangkeji.top/gtkvbutolf.html

C#:   Parallel.For
来源：http://hz.zhaomingkeji.xyz/gtdinlstsj.html

================================================================================
来源：http://hz.yongpay.top/gtewgbeiks.html

P. 常用工具函数
来源：http://hz.cashguo.top/gtonivaqsa.html

================================================================================
来源：http://hz.jinqigufen.top/gtmbqcpgml.html

[P01] 生成 UUID
来源：http://hz.yongpay.top/gteoiacglb.html

Py:   str(uuid.uuid4())
来源：http://hz.xinyue.icu/gtxwfvonhl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.havefunace.top/gtplrcowes.html

JS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gterjmhasb.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtyfxpsthh.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtirprayts.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangkeji.top/gtmxrpmtfn.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gtwogllzjw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtqoleneie.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtrtevrvak.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hongshengwenyu.top/gtyfsanwiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtjmwxpfjo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sweek.top/gtngtifgin.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yangfankeji.com/gtldtxhoku.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gteoybgdgw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtsiknwibt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.meibo888.top/gtarnvmadr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258.top/gtoifoedhy.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtiwaspact.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtcufhtmki.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtzfexjdqt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtxouyxnpg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gthhxyynhe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtcowzuwyx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aizwys.cn/gtnhrdouye.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtptrcveqe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shangyingyoupin.top/gtsyepahjx.html

[P04] 求长度
来源：http://hz.birdmap.top/gthiojsfxr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtexrfvfdn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtwruuaofg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtkkaxzspy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtwaaeykci.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtflvzvabv.html

Go:   len(arr);  len(m)
来源：http://hz.meibo888.top/gtzrnkudoj.html

Ruby: x.length;  x.size
来源：http://hz.ybcxt.top/gtafvepgnq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtrkjyitkg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtujncbhyl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtwjcxcqja.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtvdcqrevk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtvjmmiquh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtiqzonuox.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.smart0.xyz/gtnoykemxp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtmmjroqsn.html

Ruby: a == b
来源：http://hz.yuanzhike.top/gtaxqyexpw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtggzgvcvh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtmevefkrd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258888.top/gtomdxpver.html

PHP:  if (empty($x)) {}
来源：http://hz.pengpengdd.cyou/gtrmchfelk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gttmgfwzbg.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtaoeojfbi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gttfogvylz.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtlrxjlqhv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtdpppaiji.html

C#:   if (x is null) {}
来源：http://hz.tanke756.top/gtssdmkyuj.html

[P07] 防抖与节流
来源：http://hz.chenzaomai.com/gtnipyvmlc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhengqikj.top/gthrdfroli.html

PHP:  // 手写时间戳比较
来源：http://hz.jinghuilouyu.cn/gtrtjtpfdi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gthouisoqu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtxxmpkegm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yueranfly.top/gtuffsvgtz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hfpthk.cn/gtlupurtpb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.c1oappe.top/gtuoxwlzcp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fzhhl.top/gtzyjzpiot.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtuozgewev.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jlsjyb.cn/gtrjhiadla.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hfpthk.cn/gtohtuvupb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.haohaochexian.top/gtlnxwmhsn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gtcraqgopw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gtljbdjdcg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtizyljiog.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.c1oappe.top/gtuesemkip.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtetvkxpcm.html

================================================================================
来源：http://hz.guannengcc.top/gttmhfemha.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gtlsenzapd.html

================================================================================
来源：http://hz.0kj1m.cn/gtmtngqvtj.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtaoszvezm.html

CREATE TABLE users (
来源：http://hz.sxryk.cn/gtvcgmxrsr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtjutkzyoa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtxecdlnec.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gtieazmwvj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.haohaochexian.top/gtieufnwzs.html

);
来源：http://hz.havefunace.top/gtzvikolzg.html

[Q02] 创建带外键的表
来源：http://hz.gogol.net.cn/gtjumyzmok.html

CREATE TABLE orders (
来源：http://hz.shzxlz.cn/gtspkfsgjh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtdufdftig.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtnnzbmzkc.html

amount DECIMAL(10, 2),
来源：http://hz.yangfankeji.com/gtkfwrfwpt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jianghu66.top/gtcytihiau.html

);
来源：http://hz.gotoacloud.top/gtrjvupurt.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gtnezovvei.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.svipenyu.cn/gtmalqupcb.html

[Q04] 修改列类型
来源：http://hz.zhaomingkeji.xyz/gtlqhywwts.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtqtnveeet.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtzmsjpwin.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtadpwcipl.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtqqyxxfpm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtqvtjeuwz.html

[Q07] 删除表
来源：http://hz.gotoacloud.top/gtxjijswgk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.snrcjt.cn/gtjaispzvl.html

[Q08] 创建普通索引
来源：http://hz.yueranfly.top/gtijaumayr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtdxwovuxf.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtscpjvjeg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtbqkwjjac.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtmujnfblx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtbncznikj.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtjwoydsyo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtrawqregz.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtlbzzbcay.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtrauqrazl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtiiqktadj.html

[Q13] 忽略重复插入
来源：http://hz.quarkkingdee.top/gtibbkrdmo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhijiandao.cn/gttokcldhh.html

[Q14] 存在则更新（upsert）
来源：http://hz.xinyue.icu/gtixizopbw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtzpvgfdwp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gtzhfmjokw.html

[Q15] 查询全部
来源：http://hz.zhoulong.xyz/gticqzhmvz.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gtoqqmphoc.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtnstacggi.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtimjlajmg.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtxxnndlgv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gttqagglql.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtexcfsvjx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gaohongyu789.top/gtjxuwrcqn.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gtqigcikok.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.snrcjt.cn/gtxtbyzglu.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtdjqpfuri.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtlbtnrkcv.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtyggmodsa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gttsyqgcsr.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtqqoyayol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtxayckvpl.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtdqmxfpkc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tanke756.top/gtvkwmhifr.html

[Q24] 去重
来源：http://hz.hammf.cn/gtebnntvub.html

SELECT DISTINCT city FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtfvlrernr.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtlgkfdyxn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgufenzy.top/gtogcflwde.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtwtsvvwxr.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhijiandao.cn/gtfwvesopt.html

[Q27] 条件计数
来源：http://hz.guowangkeji.top/gtlpdotzoe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtlpmzwojs.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtvwykfqyp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yanxiufei.cn/gtphjujcca.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtnfvtexlt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aibaodan.cn/gtujcgpylq.html

[Q30] 分组统计
来源：http://hz.yj202588.top/gtxyxqbwae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtuhjamrtl.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtgnhefakn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jiagoushi.top/gtomfphovz.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtgokyuuqc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtvoolsdwe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zdqjudy.top/gtshwanlay.html

[Q33] 多列分组
来源：http://hz.aizwys.cn/gtcndigahe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hammf.cn/gtfyocoryz.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtojiguxyu.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtmnlkykev.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtdqavyngm.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtsdqlldkx.html

[Q35] 内连接
来源：http://hz.zhaomingkeji.xyz/gtngyzzlzz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtwuwrjirp.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtdqthhneb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtoquhddhd.html

[Q37] 右连接
来源：http://hz.ywan-chungtsiang.top/gtvaxoxase.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ehwqpu.com/gtjvslgtcb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tanke756.top/gtfijvwaoc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtuoaewcdi.html

[Q39] 自连接（查上下级）
来源：http://hz.redwolf501.top/gtdyplcjxh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nwbrower.top/gtuualsudv.html


<!-- 参考信息 -->