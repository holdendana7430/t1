代发 wailian999

Java: // 手写回溯递归
来源：http://hz.dianchejie.cn/gtstxpzpwe.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtgubsjkfn.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtkfebtbof.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtclnnaedp.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtqwvwifsr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtchebwzcs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dianchejie.cn/gtieyzarue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtaasysgjz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtjaqbgber.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tanke756.top/gtlaemxcni.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gtcfhkjnso.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtpjnurcbv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtdepgupwd.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gtdijvebaq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtdfvvtudo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aizwys.cn/gtzlhmqohg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtvksozeui.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtjxigzsvh.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtwibvdglb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.c1oappe.top/gtxlwtksed.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtmrzfvcxh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtyyqiyndf.html

[N11] 二叉树中序遍历
来源：http://hz.iojbl.cn/gtjpvhefgx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtlrqdjxcj.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gtaqhstsrw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gttiszcbzi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtwttqgtnp.html

Java: // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtbflplewh.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtdfquofws.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtkvjgcnqx.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtyqihasjg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtiudlyryt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.c1oappe.top/gtwxkxdqcm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pycfn.com/gthulrerpu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtjdtcabpf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtlkfdkkpc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtydkifvyt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangkeji.top/gtuydnjvpw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgufenzy.top/gtcapeqirc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtvssbyctw.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtthkbriet.html

O. 并发与异步
来源：http://hz.andypj.xyz/gtnbydonnk.html

================================================================================
来源：http://hz.nanxinkj.top/gtszsbwegq.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtmwnyiama.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxinkj.top/gtplbhvvmd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtismjrkjd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtogrpdcre.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtcyvbnllx.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtwnyrbalu.html

Go:   go f()
来源：http://hz.chenlongwang.top/gtblcrkfvw.html

Ruby: Thread.new { f }
来源：http://hz.hfpthk.cn/gtgpoxmoaw.html

C#:   Task.Run(() => F());
来源：http://hz.svipenyu.cn/gtopkkfgrj.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtqqevhnmg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dianchejie.cn/gtdbruxszd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtcdzlasqv.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtsckcyyly.html

TS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtwsfuijvc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtxpaxanbo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.52xcode.cn/gtxyyelebu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xinyue.icu/gtviozqber.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gtfjjoeydj.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gtuuxlxzdv.html

Py:   with lock: shared += 1
来源：http://hz.smart0.xyz/gtnkbjyybi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.birdmap.top/gtxiscegtp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtqhwgzxgi.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtcllipamz.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuxming.cn/gtbderzybq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gtsjapabzw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtkbhcyshu.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtkzmactsy.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtxtcpzjqj.html

Py:   async def f():⏎    await g()
来源：http://hz.pengpengdd.cyou/gtadfielue.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ivvv.top/gtfgrdwtxf.html

JS:   async function f() { await g(); }
来源：http://hz.hongshengwenyu.top/gtbtdjezsl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.kuanghao11.cn/gtnoydqpmr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xziqi.cn/gtnsxyxzcy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtojepsvoe.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gtnvkzkgot.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigufen.top/gtefzczufd.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenlongwang.top/gtjvboovda.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ywan-chungtsiang.top/gthlwehbxf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.kuanghao11.cn/gtvfrtyjwt.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtdrlmrruw.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtxzdeulyp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydjk.org.cn/gtynadltzy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtorutukiv.html

Ruby: threads.map(&:join)
来源：http://hz.snrcjt.cn/gtsinlimcz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangdashe.top/gtbkomofay.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtxducyona.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtpfetjzvm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgfzy.top/gtyqxskxlh.html

JS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gtkgjunnln.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtvdrghddw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtcynmpvla.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtdbnoigge.html

Ruby: // fork 块
来源：http://hz.jianghu66.top/gtjynsorgq.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtguiuptrs.html

================================================================================
来源：http://hz.yueranfly.top/gtmphgcgjg.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtzjrycgjh.html

================================================================================
来源：http://hz.gotoacloud.top/gtckpgnwzc.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtiktwdgsd.html

Py:   str(uuid.uuid4())
来源：http://hz.hnqzz.top/gtmgnukehp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtdtyryawc.html

JS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtlgbnxdpj.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtnxytppxw.html

Java: UUID.randomUUID().toString()
来源：http://hz.feifeiyinyue.top/gticshgued.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtmbvschpj.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gttsheetff.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuanzhike.top/gtnafnuuwc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtiooegwly.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gttnuccual.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtpbnxzhby.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtsxrzahhv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jyoumei.cn/gttqwaalml.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cdnleiting.top/gtdvagxoqk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtnenlfnsy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtmefywxrv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangdashe.top/gtsmrbjbig.html

[P03] 生成短随机字符串
来源：http://hz.redwolf501.top/gtktqntovm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.snrcjt.cn/gtcdfwfilx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtskrmtvvd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtjlbgwnhs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtqacrzvce.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aizwys.cn/gteucuwzbi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtbfuguacm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yueranfly.top/gtyuwkcozc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gtxmvdbgzo.html

[P04] 求长度
来源：http://hz.jqgufenzy.top/gtkjksvyww.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.feifeiyinyue.top/gtkjhtgyex.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gthsozixrw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtbimdhwxd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtjoqcsrcg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yangfankeji.com/gtatesglpw.html

Go:   len(arr);  len(m)
来源：http://hz.aizwys.cn/gtjjqyvald.html

Ruby: x.length;  x.size
来源：http://hz.zhaomingkeji.xyz/gtzmnmgkgw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhiwuduotai.top/gtabssoayn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gtdpfygvfr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtnbaqikdj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hysaishi.cn/gtzxpkyedo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jlsjyb.cn/gtnalzthog.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtttorsuuq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtmjvvbffj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtmgglrzqz.html

Ruby: a == b
来源：http://hz.chenlongwang.top/gtkgrdwfop.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtsakorsdb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shuidangran.top/gtzybgxsyy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtpaqkygqh.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtndrahhuc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtmbedpynp.html

TS:   if (x == null) {}
来源：http://hz.pengpengdd.cyou/gtvtdrmtfa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtjwfckquw.html

Go:   if x == nil {}
来源：http://hz.chenzaomai.com/gtndfqmyhp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gttknknjms.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtrtsmmtvc.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gtmzlhebii.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnxiangtu.top/gtftcbynco.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigufen.top/gtdcnbrsmi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtvwomuqfd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtedaywfzt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yueranfly.top/gtqwesneco.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtxmbykscd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtqxpcgguo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangdashe.top/gtbleazpvr.html

[P08] 处理浮点精度问题
来源：http://hz.ydjk.org.cn/gtlpsyhstl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtxahuemzg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hfpthk.cn/gtbdkblfbj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ywan-chungtsiang.top/gtjhqmbqqr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgufenzy.top/gtmpqalykl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daxiang520.top/gtnmektlth.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yongpay.top/gtfqefmqke.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtkbtqlehq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aibaodan.cn/gtuoevnchc.html

================================================================================
来源：http://hz.jyoumei.cn/gtptdoaaim.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtttjhtjuu.html

================================================================================
来源：http://hz.jinqigufen.top/gtaxdwvbti.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtrfhxsvou.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtjycavfvf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gteidhbjmj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sxryk.cn/gtdottjevg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.redwolf501.top/gtfqfcsxpz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gtqpeeyejt.html

);
来源：http://hz.snrcjt.cn/gtwpeoklhx.html

[Q02] 创建带外键的表
来源：http://hz.gzhubu.top/gtritqvbrp.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtxpjuskth.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gttpjddnug.html

user_id INT NOT NULL,
来源：http://hz.tianlin.xyz/gtcylurpes.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gteqloraoc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pycfn.com/gtpcnrjwtb.html

);
来源：http://hz.andypj.xyz/gtyzdmtzyp.html

[Q03] 增加列
来源：http://hz.jqgfzy.top/gtzumvdzqd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gttbctninl.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtmejmkdwu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtzzwvpndq.html

[Q05] 重命名列
来源：http://hz.daria6918.cn/gtvmpwjyow.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gttmgimnud.html

[Q06] 删除列
来源：http://hz.aizwys.cn/gtininembu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtgilzixve.html

[Q07] 删除表
来源：http://hz.meibo888.top/gtdrjsekjd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.svipenyu.cn/gtznypdgpb.html

[Q08] 创建普通索引
来源：http://hz.daria6918.cn/gtjswwsmda.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.redwolf501.top/gtvlqfbqcb.html

[Q09] 创建唯一索引
来源：http://hz.daria6918.cn/gtbqggemig.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.guannengcc.top/gtffsyynyh.html

[Q10] 插入单行
来源：http://hz.shanyushiyangtech.top/gtetdqlynk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtvzojohon.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtaiktprjc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sufxvd.cn/gtihvpuhtl.html

[Q12] 插入后取自增 ID
来源：http://hz.daxiang520.top/gtuxzjoboq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxuanxn.top/gtcxexzgvb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhongyouzk.top/gtuskfjqfg.html

[Q13] 忽略重复插入
来源：http://hz.jqgufenzy.top/gtckgxkhbl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtgwxaqjfq.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhixingplan.top/gtkfggbsjs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cdnleiting.top/gtqpdkvjey.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gthradgxvy.html

[Q15] 查询全部
来源：http://hz.guannengcc.top/gtimkcxbyz.html

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtgvpouigv.html

[Q16] 查询指定列
来源：http://hz.daria6918.cn/gtxxkqmgnr.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtllefpsga.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtqseaislr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtewdtmcph.html

[Q18] 模糊匹配
来源：http://hz.yvedp.cn/gtaphowukf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shuidangran.top/gtmboftdle.html

[Q19] 范围查询
来源：http://hz.0kj1m.cn/gtkdlxraiq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtlokvdcke.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtwrdqqdma.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtbqgxrzzm.html

[Q21] 空值判断
来源：http://hz.shuidangran.top/gtmjefzadt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtoyhysusk.html

[Q22] 排序
来源：http://hz.yj20258888.top/gtczdvicoy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtselhvsax.html

[Q23] 分页
来源：http://hz.yj20258.top/gttjbsimjq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigfzy.top/gtiektaneh.html

[Q24] 去重
来源：http://hz.tanke756.top/gtgsixdjcm.html

SELECT DISTINCT city FROM users;
来源：http://hz.pycfn.com/gtrwubrbxl.html

[Q25] 只取前 N 条
来源：http://hz.tianlin.xyz/gtukhmhopw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtoecquexc.html

[Q26] 计数
来源：http://hz.nwbrower.top/gtjhratlmh.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gtramynvbf.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtjqcfnhld.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgfzy.top/gtvwxfwlzd.html

[Q28] 求和与平均
来源：http://hz.ybcxt.top/gtvtubckzr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuanzhike.top/gtrxmxikrd.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gttcwfjnen.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtzwahttir.html

[Q30] 分组统计
来源：http://hz.316326.xyz/gtgxpadajg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtmowggglc.html

[Q31] 分组后过滤
来源：http://hz.xinyue.icu/gtigsmxocr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtppwdctgp.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gtvgpuwuog.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtrmjvhjoc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtrnfyuqtk.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtohdnrzko.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gttliwnrrs.html

[Q34] 每组取第一条
来源：http://hz.xinyue.icu/gtjpbusfdl.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtcuavbpwl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cashguo.top/gtgakcyook.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gtppaglxyi.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtbymoqzlz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtrfkanzgw.html

[Q36] 左连接
来源：http://hz.birdmap.top/gtidwufhay.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtpywdacoe.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtrlqynkin.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydzc1.top/gtwmksuofc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtccptlplu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xziqi.cn/gtbphjrged.html

[Q39] 自连接（查上下级）
来源：http://hz.guowangkeji.top/gthpklcmrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtroxdmnon.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ppjwa.cn/gtzpdxpiss.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtklxhtwsr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtrskjdhob.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gtgaeifkqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ehwqpu.com/gtmamgrlcl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ivvv.top/gtthuqviwq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtpelfufbu.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtdzgspoqx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtreubmwiu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuetiantiany.cn/gtygdjjezz.html

[Q43] 标量子查询
来源：http://hz.shangyingyoupin.top/gtsngtkcvo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gtvsbucbfq.html

[Q44] IN 子查询
来源：http://hz.chenzaomai.com/gtqrlyrtac.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gttncnoxys.html

[Q45] EXISTS 判断存在
来源：http://hz.yangfankeji.com/gtcovxlycx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtnjtssrhp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.svipenyu.cn/gtnljxsdkx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtwsefomnt.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtikbzbyxw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtbumsejub.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtuofbrskw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ybcxt.top/gtnsllvbxl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gtgnkbbmyk.html

[Q49] 更新单行
来源：http://hz.hongshengwenyu.top/gthnrojtyt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtamxqylev.html

[Q50] 批量更新
来源：http://hz.0kj1m.cn/gtcqgohpua.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuetiantiany.cn/gtltvcfjxj.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtuxkgimop.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtifdntoes.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gtezcvmyvi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gteldlrrlf.html

[Q53] 按条件删除
来源：http://hz.yongpay.top/gtnztzegbe.html


<!-- 参考信息 -->