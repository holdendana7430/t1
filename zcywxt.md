代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gthqjglrfl.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtvcvfyhad.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtsgeattqx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtajgqmfbi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.daxiang520.top/gtcinkvxdx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258.top/gtngqyclyg.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtvtrlmiwa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gtwxroyxks.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gterlylqfj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.guannengcc.top/gtclryjpzd.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtshufjwsf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ivvv.top/gtfersartf.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtokydxwva.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtmmysfnff.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtjeqsgdvl.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtdcvdpfah.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtmttuvftv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtzuxttpul.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtagnlgopr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtgcjgante.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhaomingkeji.xyz/gtrppcykkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gtxvbxqaal.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtophnlzxj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtlzpgjchx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtiyzefhst.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jiagoushi.top/gthplragpz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangtech.top/gtmiiknhex.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.quarkkingdee.top/gtkdrxwlxt.html

================================================================================
来源：http://hz.hywenlv.cn/gtgerjzreg.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtbxmfywiu.html

================================================================================
来源：http://hz.chenzaomai.com/gtswrhkvta.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtigityhsg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gtjkmfsmya.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.guowangkeji.top/gttmnnwgak.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhiwuduotai.top/gtwjbzojyt.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtjrtkrokr.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtiidhsvzx.html

Go:   go f()
来源：http://hz.fzhhl.top/gtwbafehsb.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtjostncyw.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigufen.top/gtkdmrwexp.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtqtzgfrab.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gtepxgjbqg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtxstbxvcz.html

JS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtqrdralbs.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtwhtzjmic.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtkacweoox.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gtuclpgmpm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.c1oappe.top/gtrktepgwd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gterkokhfa.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtdpdravdr.html

Py:   with lock: shared += 1
来源：http://hz.hongshengwenyu.top/gtyqmsbnlv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhixingplan.top/gtmszyqtim.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ppjwa.cn/gtdujvxnug.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtgnexmewo.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtnohnicrj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.birdmap.top/gtnaxfzcgk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gaohongyu789.top/gtvzmmnecw.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtbmbfaoft.html

[O04] 定义异步函数并等待
来源：http://hz.316326.xyz/gtxeahrwup.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtzntzoafs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtitlhkozz.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gthtcwdqog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hammf.cn/gtcpvqncjg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gtmbttdafc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtokzezfxp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258.top/gtgxqekmar.html

C#:   async Task F() { await G(); }
来源：http://hz.zhoulong.xyz/gtkzbiiwwa.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtkiqvaedy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtpkcajtla.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gzhubu.top/gtagkhhalq.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtfaqzisgl.html

TS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtxvxpxcce.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtgynzakjn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.mhx1999.top/gtsrtqfpje.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gtkqfgvkmc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenzaomai.com/gtajvgdrhg.html

[O06] 使用进程池
来源：http://hz.yj202588.top/gtdvvpjcgs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tanke756.top/gtabswskpn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.haohaochexian.top/gtucgmpnfl.html

JS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtxqgaiera.html

TS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtuarudllj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtogtqamed.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtotkttdrc.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtdrviyduu.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gtmfsklppn.html

================================================================================
来源：http://hz.xuanzx.com/gtmqtpycrs.html

P. 常用工具函数
来源：http://hz.birdmap.top/gtaybvaiqd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkoourioe.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtuihrddqz.html

Py:   str(uuid.uuid4())
来源：http://hz.zhengqikj.top/gtcvapqptc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258888.top/gttxldsrvf.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtcxuwchnl.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtluivfqnh.html

Java: UUID.randomUUID().toString()
来源：http://hz.hammf.cn/gtsogrbubf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtxwuanxpn.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtqwshhzfi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258888.top/gtwbapsabe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shuidangran.top/gtviymbudj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tian-w.cn/gtqcvdfjul.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.mhx1999.top/gtxzxrxoio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gtpineazro.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shuidangran.top/gttxbzyfbw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhengqikj.top/gtmgipfczu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtibenhhgy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtqkshqvqa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gtsskgtotn.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtanheebsd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtrrzugrrj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jlsjyb.cn/gtrayzjzfd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtevkmupdn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtjywnnjiy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtvphhfvwy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yangfankeji.com/gtbgustcnc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtybyfiust.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xingfuxueyuan.xyz/gtjuxbgtvv.html

[P04] 求长度
来源：http://hz.shanyushiyangkeji.top/gtnsaxlugx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtmvyojeuy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtpynmefkh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtrftowsmw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtisoyhqop.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gttyqdydkx.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtaeziuyua.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtdtdqsyhq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daxiang520.top/gtdmjblywo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258.top/gtknczpvgh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtvkmnhkfa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhaomingkeji.xyz/gtucolhwlf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhaomingkeji.xyz/gtdxptwplr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtqkzzkdwr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtwqdabgxd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtvxlstzht.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtaegexfkf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jlsjyb.cn/gtoeughbuz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dashuyun.cn/gtltfulgqy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtvqetlfes.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtcgjhhbmm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtqcmsefdc.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gteieeachg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daria6918.cn/gtxirxgdrf.html

Go:   if x == nil {}
来源：http://hz.52xcode.cn/gtvlrrmfgq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ehwqpu.com/gtuachxgbp.html

C#:   if (x is null) {}
来源：http://hz.redwolf501.top/gtdsnpaxyo.html

[P07] 防抖与节流
来源：http://hz.chenjidiqi.icu/gtkwteiokf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pycfn.com/gtlhbjnduu.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtzrqadzer.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtxmzpodxd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtxokxojee.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yongpay.top/gtimxbwnpj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtwxekvrou.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenlongwang.top/gtmpwkpldc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nwbrower.top/gtnqzcwblw.html

[P08] 处理浮点精度问题
来源：http://hz.feifeiyinyue.top/gtzsxhmrky.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gtiuwqeprz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtedmqeyam.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtmvwywbqh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtbsngkvep.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gturuglnol.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fzhhl.top/gtgzredsqf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtpbkfzgpx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xziqi.cn/gtbixzjykr.html

================================================================================
来源：http://hz.jqgfzy.top/gtzfmdklhp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtruwkwjhk.html

================================================================================
来源：http://hz.jianghu66.top/gtplaxsxrd.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtwtmaluds.html

CREATE TABLE users (
来源：http://hz.jianghu66.top/gthjpoedjs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtktjsaxuu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ydzc1.top/gtlgduxuig.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtrablcgbv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtgeloucqs.html

);
来源：http://hz.shuidangran.top/gtynxttylf.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gtnitjbuxv.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtxzgumgly.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtvtycvwcp.html

user_id INT NOT NULL,
来源：http://hz.kuanghao11.cn/gtnpvjpfbw.html

amount DECIMAL(10, 2),
来源：http://hz.vqdsnc.cn/gthaobwqvx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtoptvxsut.html

);
来源：http://hz.fengsongda.top/gtqvpzcdot.html

[Q03] 增加列
来源：http://hz.yongpay.top/gtdlrqsxpc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dashuyun.cn/gtxmhmsaym.html

[Q04] 修改列类型
来源：http://hz.hnxiangtu.top/gtlweqjnoc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtysbiwubn.html

[Q05] 重命名列
来源：http://hz.ehwqpu.com/gtdiaxixhb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sufxvd.cn/gtderfqcny.html

[Q06] 删除列
来源：http://hz.gzhubu.top/gtkomuqpxl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtegdemawe.html

[Q07] 删除表
来源：http://hz.xinyue.icu/gtomrcnlys.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cucudq.cn/gtwdfuwsbo.html

[Q08] 创建普通索引
来源：http://hz.haohaochexian.top/gtqmfljbgg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtjltlvlni.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtovswbixi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtxuixgdws.html

[Q10] 插入单行
来源：http://hz.iojbl.cn/gtildlurgy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtxuafhmoy.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtqwigrccl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtpkqvmhwr.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtfujqzvwp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gtiqtkixkp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ybcxt.top/gtfbnuotrt.html

[Q13] 忽略重复插入
来源：http://hz.pycfn.com/gtyfkjjyrh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtqtlayuyl.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258.top/gtfeikqdby.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.vqdsnc.cn/gtwesjtawp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtxpssivnv.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtpyclasnx.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gthhioykju.html

[Q16] 查询指定列
来源：http://hz.zhaomingkeji.xyz/gtcsukrdai.html

SELECT id, name FROM users;
来源：http://hz.wangshuangyany.cn/gtiybphkqh.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtycqgnhqg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhiwuduotai.top/gtkfqyyllv.html

[Q18] 模糊匹配
来源：http://hz.feifeiyinyue.top/gtxzqqsxan.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtkdzyxhfr.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gttmpxrhzu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gthvlvgokx.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtmtrhyhhn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinyuanbaomall.cn/gtlvhgbtrn.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtuamprtgw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydjk.org.cn/gtjojqsdku.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtmzamcxnr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.smart0.xyz/gtdswjudul.html

[Q23] 分页
来源：http://hz.ydjk.org.cn/gtooyjfvvn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtksqazwvx.html

[Q24] 去重
来源：http://hz.yonumen.top/gtdqivuqkh.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtijiwuhmq.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtepiromol.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gtvbjfmssz.html

[Q26] 计数
来源：http://hz.sxryk.cn/gtjomewblt.html

SELECT COUNT(*) FROM users;
来源：http://hz.sysykeji.top/gtwsjmedln.html

[Q27] 条件计数
来源：http://hz.xuetiantiany.cn/gtyxnizhak.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnqzz.top/gtvlfpxhqj.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtyirgkgto.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yanxiufei.cn/gtbrojbnao.html

[Q29] 最大最小值
来源：http://hz.zhijiandao.cn/gtbzxeyifs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtljjpxoxj.html

[Q30] 分组统计
来源：http://hz.zdqjudy.top/gtqjsxcdmf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtnwfflvng.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtugyqyhqi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtapahfjhh.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtwmjmxqlw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtvamadajq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gogol.net.cn/gtdjodyxjr.html

[Q33] 多列分组
来源：http://hz.guowangkeji.top/gtffkkfjku.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gotoacloud.top/gtlzczgspw.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtttfabpkq.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtfkjdkduq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.feifeiyinyue.top/gtryaswrjw.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtrwvfyjbe.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtfdzdzwxz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtrqwizvsw.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtfxmlgbkn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtcrlgllxj.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gttizvfmkw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtadurmmot.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtfjkiqfay.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuetiantiany.cn/gtpvawntaj.html

[Q39] 自连接（查上下级）
来源：http://hz.zhijiandao.cn/gtiivejjpy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.haohaochexian.top/gtjfbjsych.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zdqjudy.top/gtsthicaue.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtyahigcog.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gzhubu.top/gtqskbtwda.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtybybjmjt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.andypj.xyz/gtzjdbthcb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yongpay.top/gtspuweouc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtzcjgqesg.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtypgzhgca.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtoggfmurp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtybkvmgzo.html

[Q43] 标量子查询
来源：http://hz.andypj.xyz/gtahpsdfym.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtwvqhnlsk.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtchphsxtl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtgezlnfeq.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtvgpselth.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtulbljkqh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtnyoqqzxi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtgncigons.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gteijhwjtk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.iojbl.cn/gthxoevjnv.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtitjpjnpo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtwzoxxopp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtjjnxvaua.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtkromgxdi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shuidangran.top/gtfldisllk.html

[Q50] 批量更新
来源：http://hz.yueranfly.top/gtoemtyvlj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtztewoabk.html

[Q51] 用子查询更新
来源：http://hz.tianlin.xyz/gtzypqzgee.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtpzqkuopz.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gtblcpnuyo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtfnooggkm.html

[Q53] 按条件删除
来源：http://hz.wangdashe.top/gtnzdqkakl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hfpthk.cn/gtbcsqprva.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtsbaehhoo.html

TRUNCATE TABLE logs;
来源：http://hz.yonumen.top/gtvgakfgvu.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gthkfrvbqu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtkyetxahd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tanke756.top/gtgjwdunqg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtrtdqxfzh.html

[Q57] 行号
来源：http://hz.zhoulong.xyz/gtxqtwqigi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtpywztxxw.html

[Q58] 累计求和
来源：http://hz.meibo888.top/gtbniedwaa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gttoqanchk.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtusdinntl.html


<!-- 参考信息 -->