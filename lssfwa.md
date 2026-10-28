代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.jqgufenzy.top/gtnjtwgmrb.html

PHP:  // 手写递归交换
来源：http://hz.daxiang520.top/gtrmvuczyl.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gttfdwcrfm.html

TS:   // 手写回溯递归
来源：http://hz.sweek.top/gtxwgvgwwq.html

Java: // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtnallhjpu.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtbswwmjna.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gthuuetcce.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtoupkohyd.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gteyjmvbsr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtjqwxsfjq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gtjktrmrpg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtjummqkmq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hfpthk.cn/gtskvrprxg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtnhtmlgzf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dashuyun.cn/gtgodsfkqd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtkertnoxo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtygappyqc.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtyzsyjiuu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtlhjynyyf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtsfqavzka.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtjxyjjadu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtwvkcmnpo.html

Java: class Node { int v; Node next; }
来源：http://hz.jinghuilouyu.cn/gtfeesdwhm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guowangkeji.top/gtihgecbil.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenlongwang.top/gtbcffcwko.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtlajluucb.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtlaqfcsss.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtvhbbaozv.html

PHP:  // 手写递归函数
来源：http://hz.zhijiandao.cn/gtdehisvmy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtphfurlcy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtracghwsy.html

Java: // 手写递归
来源：http://hz.snrcjt.cn/gtiajuxmgb.html

Go:   // 手写递归
来源：http://hz.jqgufenzy.top/gtbmfymkgh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ywan-chungtsiang.top/gttysjoyuo.html

C#:   // 手写递归
来源：http://hz.kuanghao11.cn/gtzrqmafif.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.mhx1999.top/gtiybfjryj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cheryme.top/gtouvocymw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gtddxirtko.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtmhfhfeyr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtafjdkyfn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtvwpgybwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtplymuzqb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guannengcc.top/gtgfrhoftv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtwcjmprem.html

================================================================================
来源：http://hz.gotoacloud.top/gtxwckdqml.html

O. 并发与异步
来源：http://hz.daria6918.cn/gtdnhwmhzt.html

================================================================================
来源：http://hz.dianchejie.cn/gtljmrmsfw.html

[O01] 启动一个线程
来源：http://hz.jqgfzy.top/gtpayfdqcy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtmyejbcim.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gtairibihh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yongpay.top/gtbkshknef.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtoabisptt.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gtoizxnqzq.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtinzeeiol.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtxofacnav.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtfaospent.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gtsmzxeexe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtovrpcvpi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.316326.xyz/gtwwwelyja.html

JS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gteivpeqxy.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtkmbmynfx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xuanzx.com/gthidvezob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtijjbtozi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ivvv.top/gtqulpbxzu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtyzhpqblk.html

[O03] 加锁保护共享数据
来源：http://hz.shzxlz.cn/gtygcdbqyv.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtadzegagf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtegijlifp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.feifeiyinyue.top/gtbtpzqbba.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtsnjupejj.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtofbvgzrr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangshuangyany.cn/gtrcrytvxp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtinzwxavp.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtxzadzquj.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtqzabsllc.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtrrhdpspp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.svipenyu.cn/gtsfivhiis.html

JS:   async function f() { await g(); }
来源：http://hz.pycfn.com/gtcnuitozz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtnigpjsqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtefbuaevi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtxmlckevm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtrlnheeou.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtaoaewuij.html

[O05] 并发执行并等待全部完成
来源：http://hz.cheryme.top/gtorcacdlo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tianlin.xyz/gtlcblqywp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yongpay.top/gtwouaqunc.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtatwvloms.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtzppuhgrr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gttmdzpxim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtauksqvpf.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtiegkbsoh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtwnfnxjxd.html

[O06] 使用进程池
来源：http://hz.chenzaomai.com/gtxzgkkine.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guannengcc.top/gtbiqsypdg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtqtwduddd.html

JS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtnsxddcqw.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtpqxhqqwj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtvvynzshp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtceafwngr.html

Ruby: // fork 块
来源：http://hz.mhx1999.top/gtmbclmnok.html

C#:   Parallel.For
来源：http://hz.sweek.top/gtegucnwjo.html

================================================================================
来源：http://hz.zhengqikj.top/gtbaotjarx.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtzptyrbwm.html

================================================================================
来源：http://hz.hammf.cn/gtzwqaqndk.html

[P01] 生成 UUID
来源：http://hz.yj202588.top/gtyozybgbc.html

Py:   str(uuid.uuid4())
来源：http://hz.chenjidiqi.icu/gtpqtzlaze.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gtssgmzpsc.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtepqzjpsl.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtgxmzvqfg.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtgpsdhtum.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtvzmwicip.html

Ruby: SecureRandom.uuid
来源：http://hz.andypj.xyz/gtotxunoen.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sysykeji.top/gtpumjgoqp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtebldzjza.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtopkigjfq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtxmwimrha.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.feifeiyinyue.top/gtcqpfzoii.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zycfv.cn/gtpscirgep.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xylfe.cn/gtmavgzyiu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gtjohhnlpq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtqjgxkjmr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtnrawclze.html

[P03] 生成短随机字符串
来源：http://hz.gogol.net.cn/gtdasitbiz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtwrqrppvb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tian-w.cn/gtnsedmbjp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtvxujqbdo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtehmuvrts.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinyuanbaomall.cn/gtmrcxrxoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinqigufen.top/gtoqjmppgk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtoovizlwv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.vqdsnc.cn/gtkobhqioe.html

[P04] 求长度
来源：http://hz.316326.xyz/gtyzhqosoa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhengqikj.top/gtoivclfgx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gthaowwaxw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtpgtwnfru.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtptkwfwqu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hfpthk.cn/gtdrgzgwej.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtjlmyftfd.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtargktbrn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.svipenyu.cn/gtjqtojetp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.birdmap.top/gtmivisirs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gttyghptcw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhoulong.xyz/gtptlotrpz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.kuanghao11.cn/gtlvazrmvz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtrffvipvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtajlfdgkl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sxryk.cn/gtpifvoswg.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtocmaenav.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtgquinykn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtezpgsutb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gtojdvwlbl.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtguzprpfr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sysykeji.top/gtecpnrwun.html

TS:   if (x == null) {}
来源：http://hz.gaohongyu789.top/gtnwnxwjmo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtvkgdwsag.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtjpkfokhc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtqqenhehv.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gtwghodqfe.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtneadomhe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nwbrower.top/gtazknzhuz.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtflauszoq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtwoxsmgqo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtkbwaeomn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtmdbeyxmw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtvyjzvxjf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinyuanbaomall.cn/gtyyrgijrs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hysaishi.cn/gtutntspdv.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtyeosditq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtquitspvy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dashuyun.cn/gtbhnycktk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gtfetloymw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.svipenyu.cn/gtadxcvanl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtmtbmspqw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.havefunace.top/gtksfkbwvn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinghuilouyu.cn/gtovlgqvda.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtsbemtien.html

================================================================================
来源：http://hz.daxiang520.top/gtbldisgmc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gtmlsyyoek.html

================================================================================
来源：http://hz.snrcjt.cn/gtiteebfqf.html

[Q01] 创建表
来源：http://hz.zhoulong.xyz/gtmyinndpq.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtypxhezsr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtysofgsuv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jlsjyb.cn/gtlxbgqxgy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtemcfuxhk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.andypj.xyz/gtdftuchsi.html

);
来源：http://hz.yj20258.top/gtewixdtvv.html

[Q02] 创建带外键的表
来源：http://hz.gaohongyu789.top/gtydrmsxhi.html

CREATE TABLE orders (
来源：http://hz.jianghu66.top/gtqdqkgcvz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gthipsoepa.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gthslipcli.html

amount DECIMAL(10, 2),
来源：http://hz.jlsjyb.cn/gtjdobuwvn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtbynjunoq.html

);
来源：http://hz.guowangkeji.top/gtrzzrljim.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtrwknjenp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtzdlwerhq.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gtgqdenmim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhijiandao.cn/gtycnviriu.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtuviejsbu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xingfuxueyuan.xyz/gtwhkwgpkc.html

[Q06] 删除列
来源：http://hz.gotoacloud.top/gtefsebozl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guannengcc.top/gtelpqyeoz.html

[Q07] 删除表
来源：http://hz.nanxinkj.top/gtnmupcblt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtrnrswdzk.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtkvihtahs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xylfe.cn/gtfabwwkja.html

[Q09] 创建唯一索引
来源：http://hz.hnqzz.top/gtiaxhlphn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtdednhwvy.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtgnbpktmn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtgtpeywkh.html

[Q11] 一次插入多行
来源：http://hz.hnqzz.top/gtddbsftfg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtiutivewl.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtulnjatjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xziqi.cn/gttvxizzta.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yvedp.cn/gtdlrnwlul.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtfqqcshmy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xziqi.cn/gtwsjlbcsl.html

[Q14] 存在则更新（upsert）
来源：http://hz.0kj1m.cn/gtmzlcgwqe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtxawoaqwe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xziqi.cn/gtmymcmakz.html

[Q15] 查询全部
来源：http://hz.andypj.xyz/gtlyedkrnq.html

SELECT * FROM users;
来源：http://hz.zhiwuduotai.top/gtoshptglq.html

[Q16] 查询指定列
来源：http://hz.zhoulong.xyz/gtxgiflmlg.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gtcpakwvrg.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtowgibpcv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtdfwarqid.html

[Q18] 模糊匹配
来源：http://hz.yangfankeji.com/gtpvexfcsa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtzqsodozg.html

[Q19] 范围查询
来源：http://hz.ywan-chungtsiang.top/gtecbnxkjx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tian-w.cn/gtyyoaayva.html

[Q20] IN 列表
来源：http://hz.yuxming.cn/gtwylmpbwp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtofkhuyyc.html

[Q21] 空值判断
来源：http://hz.shangyingyoupin.top/gtcncxherg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgufenzy.top/gtdtiztdfv.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtxyvhharx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.havefunace.top/gtfilqwypx.html

[Q23] 分页
来源：http://hz.mhx1999.top/gtkebtaoax.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.snrcjt.cn/gtivkstaup.html

[Q24] 去重
来源：http://hz.kuanghao11.cn/gtrcjanjpj.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtohgsmhbo.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtlkdwztoi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtqcqwtsws.html

[Q26] 计数
来源：http://hz.yanxiufei.cn/gtvubrexaa.html

SELECT COUNT(*) FROM users;
来源：http://hz.9152youxi.cn/gtoapxeliz.html

[Q27] 条件计数
来源：http://hz.jinghuilouyu.cn/gtjjsmkfsj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangshuangyany.cn/gtewqguegp.html

[Q28] 求和与平均
来源：http://hz.sweek.top/gtifaapdic.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yongpay.top/gtwkttmige.html

[Q29] 最大最小值
来源：http://hz.haohaochexian.top/gtwyivrcja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtrxlqmyzd.html

[Q30] 分组统计
来源：http://hz.52xcode.cn/gtdnavhtus.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtfzjqiuuh.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtvxsrhlse.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jianghu66.top/gtmhgdmioo.html

[Q32] 分组拼接字符串
来源：http://hz.cqqwz.cn/gtzksjaktf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtyowrpkid.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtjvmhjeuc.html

[Q33] 多列分组
来源：http://hz.shangyingyoupin.top/gtjzqdgmwn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.birdmap.top/gtgspqcgwg.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtpokauepj.html

SELECT * FROM (
来源：http://hz.yangfankeji.com/gtjhxkshkm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258888.top/gtjefqxhdf.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtaqbwxiqf.html

[Q35] 内连接
来源：http://hz.zycfv.cn/gtokhfkrch.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtimwwshjx.html

[Q36] 左连接
来源：http://hz.cashguo.top/gtgshlasmy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtzmyjrzrq.html

[Q37] 右连接
来源：http://hz.yuxming.cn/gtdzcmihkf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.andypj.xyz/gtkvktdqia.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dashuyun.cn/gtajalfmdg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtamdesgyx.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtbcrnqlad.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shangyingyoupin.top/gtonvjnuyk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtflionavz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtijmzohaz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gteilixepr.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtpdxnezxa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtfhahqhfo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nwbrower.top/gtfkjckovo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gtgrakkkrh.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtksuqgvao.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtffaicfuc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gtbpwskmvl.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtyjpnuepv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtkzklkedc.html

[Q44] IN 子查询
来源：http://hz.yueranfly.top/gtuqulfdqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pengpengdd.cyou/gtqgmbzbnm.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtkzqhizue.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtpzfxlpsh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhijiandao.cn/gtuxdghycc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtbmxxeiht.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtjhksppcm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnxiangtu.top/gtsdtpztgi.html

[Q48] CTE 公用表表达式
来源：http://hz.fzhhl.top/gtgqjpugoh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtyfdfexve.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zdqjudy.top/gtjlmzmtcy.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtvhdbkpbj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tianlin.xyz/gtcannwedh.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtlnlegqil.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.vqdsnc.cn/gtfxlndonu.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtknjpvibh.html


<!-- 参考信息 -->