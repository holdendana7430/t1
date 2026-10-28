代发 wailian999

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gtvewnpvyx.html

Go:   // 手写回溯递归
来源：http://hz.yj20258.top/gtssvyehur.html

Ruby: arr.permutation.to_a
来源：http://hz.fzhhl.top/gtdxtrajpm.html

C#:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtfpsdrwif.html

[N09] 栈与队列
来源：http://hz.jqgufenzy.top/gtkqveqlwp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hammf.cn/gtytqwvgoo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jyoumei.cn/gtltrgymgj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtrlbxlbqs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gotoacloud.top/gthvhrlsny.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cucudq.cn/gtazaelzoh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtzxnygfto.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jyoumei.cn/gtllmswson.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtttxbnyyw.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtsyozxccl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtzsbzetgg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yvedp.cn/gtoogexxtz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.havefunace.top/gtkvlqczrq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtovugjvlg.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtyruldspl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangtech.top/gtdenptyxn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.svipenyu.cn/gtlcqprlbw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydjk.org.cn/gtjavztnpt.html

[N11] 二叉树中序遍历
来源：http://hz.shuidangran.top/gtdhsfjpgj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtitmhkqka.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtcqricybp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtrmiferqq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtfgrdllvt.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtktpmhsdg.html

Go:   // 手写递归
来源：http://hz.pycfn.com/gtfyozzbdg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.mhx1999.top/gthapdukfd.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtmoylvfvi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtcgqtsbrx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gtotdlcdcm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gtfgigprig.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtlmhilpyn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtwxfynzma.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtbeidkmhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuetiantiany.cn/gtquautbhg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenlongwang.top/gtztbhnqoo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gtltsujgvj.html

================================================================================
来源：http://hz.cheryme.top/gtojjagvgd.html

O. 并发与异步
来源：http://hz.yonumen.top/gtczyqsian.html

================================================================================
来源：http://hz.cheryme.top/gtsihzdswn.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtsdxjusnj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tianlin.xyz/gtcmhyxsvc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtkjytyxrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtbkckzuzr.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtgjzlmjxd.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtqvhjdfeo.html

Go:   go f()
来源：http://hz.9152youxi.cn/gtliguzanv.html

Ruby: Thread.new { f }
来源：http://hz.c1oappe.top/gtvirkexmd.html

C#:   Task.Run(() => F());
来源：http://hz.yanxiufei.cn/gteenpochj.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gthtrizjmv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtwprljqfx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.9152youxi.cn/gtircmnzsj.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtmwvneoqs.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtdamkkflp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtvcokdhpn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxinkj.top/gtakczqxje.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtcgphvkds.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtvzxgexac.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtjkrbagoe.html

Py:   with lock: shared += 1
来源：http://hz.zdqjudy.top/gtrlxlwddv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gtkfdllkcd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtjcjkfftw.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtmrrhmxcm.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtgfggyyiy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtzsgbuhkr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yanxiufei.cn/gtxfqedsgi.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gtsoyzpnyw.html

[O04] 定义异步函数并等待
来源：http://hz.jianghu66.top/gtchwdfqtn.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gtzjnkfqeu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtznbxutsz.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtrpmczicz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gzhubu.top/gtiinlwhwu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.c1oappe.top/gtjyfcfsaj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtzjisqgux.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtdtpbildq.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtrhbkrubu.html

[O05] 并发执行并等待全部完成
来源：http://hz.yanxiufei.cn/gtdpveqmwr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.9152youxi.cn/gtolitajmn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydjk.org.cn/gtslhxcfux.html

JS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtthsjsafz.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtmgyiycpp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cqqwz.cn/gtlztecuvp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtvljevpeo.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gtklwoudvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gteqewnotz.html

[O06] 使用进程池
来源：http://hz.sufxvd.cn/gtrnuvubpx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtxsqlfqmm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pengpengdd.cyou/gtqxzwjmpz.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtgztquzvj.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtrcmeibkq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtuyftunfn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtabplclwc.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtceferfzp.html

C#:   Parallel.For
来源：http://hz.shangyingyoupin.top/gttacmjxwq.html

================================================================================
来源：http://hz.pycfn.com/gtnxkgndcj.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtrmxelpoa.html

================================================================================
来源：http://hz.fzhhl.top/gtggpuvivw.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtbhnzebcu.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gtqxcvzale.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cdnleiting.top/gtvazccxpz.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtcigiuiav.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtreovfpgn.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gteqitbwqk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.mhx1999.top/gthodopket.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtjatebzrv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.meibo888.top/gtxkvijwiw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtqgxqfeqw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtatmrwuoq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yangfankeji.com/gtksmerben.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtaxdypxma.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.316326.xyz/gtmgjhuytc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtwfovdxjc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gttxyhjves.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.quarkkingdee.top/gtclcvfshk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guannengcc.top/gtwlyekams.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gtwwlhzonf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ywan-chungtsiang.top/gtpfgqjlap.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtvrepxeel.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtjppftjvq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gthowbsmqd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtwwvnocad.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtlotxojqj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtalwnrslz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtoallkoim.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtphmmeheh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gthiurhobo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtkzgwaari.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgfzy.top/gtxdulxpfm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtkgknmfzo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shzxlz.cn/gtxhfewcxb.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangtech.top/gtjemepgdl.html

Ruby: x.length;  x.size
来源：http://hz.jiagoushi.top/gtzmzrxapt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtfppficfz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtteogjohv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtmlayspaa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtplreotea.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jianghu66.top/gtmijikllu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtkpoxtpfa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nanxinkj.top/gtcvopvqbc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.mhx1999.top/gtclfdxbus.html

Ruby: a == b
来源：http://hz.gotoacloud.top/gttqbucjnc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gthynlghci.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhijiandao.cn/gtcjflhgmz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtvhetmrse.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gthwtfxcvg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gttpoyibcz.html

TS:   if (x == null) {}
来源：http://hz.zycfv.cn/gtnwcebasj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yueranfly.top/gtpyrhqjkz.html

Go:   if x == nil {}
来源：http://hz.tanke756.top/gtitlzyupe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.svipenyu.cn/gtdhythcdb.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gtgmkkagkq.html

[P07] 防抖与节流
来源：http://hz.kuanghao11.cn/gtjygsdymp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shuidangran.top/gtokzxxfbf.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtgbvmfrmm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtcmolweuc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gttyojfpab.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtyvpgruyc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtibschhru.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gogol.net.cn/gtvuvvojqo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinyuanbaomall.cn/gtbxcycjfm.html

[P08] 处理浮点精度问题
来源：http://hz.sufxvd.cn/gtlpniyfcx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtsfdybnaz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj202588.top/gthoedkruy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yongpay.top/gteidghdos.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtiuillwox.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinghuilouyu.cn/gtelxargnr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ivvv.top/gtnnijzkdw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtywhvitqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtdntsdnao.html

================================================================================
来源：http://hz.zhengqikj.top/gtbqmicund.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.andypj.xyz/gtrovnfiwi.html

================================================================================
来源：http://hz.andypj.xyz/gtkfkdsxah.html

[Q01] 创建表
来源：http://hz.nanxuanxn.top/gtdgzmrupq.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gttwrkzard.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtpeeowtsq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtzykuucpu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gtfhdtdche.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtkfzegpqk.html

);
来源：http://hz.tianlin.xyz/gtgxuzxjeo.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtvlylmuqt.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtbylogfxs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtxlapjokn.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtmpzdxpql.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtjvhwsawi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtkjetmtmq.html

);
来源：http://hz.jinyuanbaomall.cn/gtkeesyqzi.html

[Q03] 增加列
来源：http://hz.shanyushiyangkeji.top/gtkviliupf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daria6918.cn/gtlqfcblqi.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gthnjpxkpi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtsvwjeprt.html

[Q05] 重命名列
来源：http://hz.smart0.xyz/gtxjhhkpvv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gttsapkxmd.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtlmomjovg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuanzhike.top/gtuaekdsyq.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtgeedmswj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gthfpmtzgo.html

[Q08] 创建普通索引
来源：http://hz.zhiwuduotai.top/gtqhbzplsj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnqzz.top/gtxkvjcyso.html

[Q09] 创建唯一索引
来源：http://hz.tian-w.cn/gtjfqkbxjw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtxgrmwixl.html

[Q10] 插入单行
来源：http://hz.shanyushiyangtech.top/gtrzcktign.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtphndzetu.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gteufupall.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtkfgonten.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtnnrdbqhy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtgegvwtgh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.quarkkingdee.top/gtybrbpcrk.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtnhhacvbt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aizwys.cn/gtrvsyicgj.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtuwlfuibq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yangfankeji.com/gtubetzmsq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtpzhmueol.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtfpepwkhy.html

SELECT * FROM users;
来源：http://hz.aibaodan.cn/gtljzzubdy.html

[Q16] 查询指定列
来源：http://hz.sysykeji.top/gtsxzjbocf.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtgaxhlvdp.html

[Q17] 条件查询
来源：http://hz.316326.xyz/gtbijaxlbf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sxryk.cn/gtmlnpeeae.html

[Q18] 模糊匹配
来源：http://hz.fengsongda.top/gtzebyqodz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnqzz.top/gtvmloxdsz.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gtshmkexmu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.bjfxy.top/gtzegulazz.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtysqosvqj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xinyue.icu/gtwutknane.html

[Q21] 空值判断
来源：http://hz.yonumen.top/gtsqjtjwlp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtsyxcszjh.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtnegjcuvd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtqznmawbv.html

[Q23] 分页
来源：http://hz.guowangkeji.top/gtyskmwdjn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jlsjyb.cn/gtdfdgmamy.html

[Q24] 去重
来源：http://hz.tanke756.top/gtezmllmjs.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinghuilouyu.cn/gtiggcxzue.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtgqckrlkk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgfzy.top/gttutewmsj.html

[Q26] 计数
来源：http://hz.shuidangran.top/gtpahvagki.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtrpefsbco.html

[Q27] 条件计数
来源：http://hz.hfpthk.cn/gtqanotyep.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhijiandao.cn/gtriuxozyv.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtekacpshv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gttyfqiomt.html

[Q29] 最大最小值
来源：http://hz.jqgufenzy.top/gtgibkbrjb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cucudq.cn/gtzwgeuqxs.html

[Q30] 分组统计
来源：http://hz.zdqjudy.top/gtwinoynpu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gthvpevkkc.html

[Q31] 分组后过滤
来源：http://hz.0kj1m.cn/gtmyvuqopa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtfgjyottw.html

[Q32] 分组拼接字符串
来源：http://hz.cashguo.top/gtluflfjah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtoaancfzz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cheryme.top/gtzertvvxn.html

[Q33] 多列分组
来源：http://hz.ppjwa.cn/gtfmfocnza.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gthliidpso.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtsrthptap.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gthalpmhgn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtbxicdqiq.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtbbnnzsgb.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtdaduuhrk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtvnbvsorb.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtswsthuwy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtsfwunaxy.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gtcqtoeoow.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuxming.cn/gtztncbbsb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ybcxt.top/gtyjprkakh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gtnwnrbxwe.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtfcwxykbj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtsgmhmdxw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtsbevkexu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtsdhacdzq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtoyewpgxx.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtwbehhxqy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtxsqnzkba.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtkjamkimv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.haohaochexian.top/gtlasvyakr.html

[Q42] 连接条件附加过滤
来源：http://hz.haohaochexian.top/gthwvolmdy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtfjusznqt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gttvcqyhlf.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gtpyawaspy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhijiandao.cn/gtpqaiknyi.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtkurczqlb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.c1oappe.top/gtnrlttkdq.html

[Q45] EXISTS 判断存在
来源：http://hz.iojbl.cn/gtevqnvaqt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtfypkcejc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shangyingyoupin.top/gtpkfbpjqf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtvjuqtjvp.html

[Q47] 与平均值比较
来源：http://hz.cucudq.cn/gttvkeuphs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhongyouzk.top/gtqtopswbg.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtwxlfyjxj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtdeedwzig.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.feifeiyinyue.top/gtbjjrseux.html

[Q49] 更新单行
来源：http://hz.sysykeji.top/gtlgoyxcma.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sxryk.cn/gthzrlgbpk.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtikwaeqvw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gogol.net.cn/gtvovdfurd.html

[Q51] 用子查询更新
来源：http://hz.hywenlv.cn/gtlozrqzhe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.52xcode.cn/gthcafnvpw.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtvblzkmtp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtpvnsufol.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gtdmfumady.html


<!-- 参考信息 -->