代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtxktqiwhk.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtjmoymbjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ybcxt.top/gtbqtimnoe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtknufvvtk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangkeji.top/gtyqubwshp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ywan-chungtsiang.top/gtkjaeuxvn.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtyhqftwpa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yongpay.top/gtqkbwvzix.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fzhhl.top/gtklrilnse.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtpwnwbrpq.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtwbzlgqnl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenjidiqi.icu/gtalzqqmbx.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtglghpgzx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtlpdckyjo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtpploycag.html

Java: // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtxzjnpoqy.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtjxdczhyu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtptlorynm.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtmockvvuf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtqnzwacbl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gttwkyxnlp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenjidiqi.icu/gtattwcizp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtztroybrp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtoxieporc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtcvoikvqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtuvkkdrig.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cdnleiting.top/gtdsuleazc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtrzhxaykq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmmhabkbn.html

O. 并发与异步
来源：http://hz.ydzc1.top/gtvkcevdbh.html

================================================================================
来源：http://hz.gzhubu.top/gtdyhisefu.html

[O01] 启动一个线程
来源：http://hz.hysaishi.cn/gtivlpfdxl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.svipenyu.cn/gtammvsmvn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gtwtkdfupu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhiwuduotai.top/gtmdinaezw.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtjytgoedi.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtaltdcxcs.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtpptrzkkc.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtvieyesen.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtbkdeqeon.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtghgahtir.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtintmjyfx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtyvilcjcr.html

JS:   // worker_threads 线程池
来源：http://hz.jianghu66.top/gtnsgdsosh.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtlbuoitar.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtzfjrnxqr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gtrzhqbjep.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dashuyun.cn/gtmvtfafor.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtohavkggn.html

[O03] 加锁保护共享数据
来源：http://hz.yueranfly.top/gtwalaqtfg.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtjklwgvnq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtuqzhjdyo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtffyhbmgn.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtyoovrrjb.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtlxcuzxbb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenjidiqi.icu/gtvkdpngdt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gzhubu.top/gtiiwarbjz.html

C#:   lock (gate) { shared++; }
来源：http://hz.hywenlv.cn/gttidxplyy.html

[O04] 定义异步函数并等待
来源：http://hz.svipenyu.cn/gtuobblzzm.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtblkfslqy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtczzhwuzn.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtqpkfdnod.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cheryme.top/gtqqnzdokj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenlongwang.top/gtvmgkjttp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtjazghpml.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtorapdwjs.html

C#:   async Task F() { await G(); }
来源：http://hz.fzhhl.top/gtfadizvxm.html

[O05] 并发执行并等待全部完成
来源：http://hz.9152youxi.cn/gtzfhvfmms.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxuanxn.top/gtnlfehdbz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.9152youxi.cn/gtosfkwqhp.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtxpdqfcqh.html

TS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtueerrbcd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xziqi.cn/gtpisrgtot.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtzwxzszbo.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtifdsfvit.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj202588.top/gtqszpwpkp.html

[O06] 使用进程池
来源：http://hz.ppjwa.cn/gtgctynoze.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gtarhnwnvi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtjigswjfd.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtzratjjsk.html

TS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtlwymyeqm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gogol.net.cn/gtbnderrny.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tanke756.top/gtlfepbhdp.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gttjytpxwy.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtsxrzihkz.html

================================================================================
来源：http://hz.daria6918.cn/gtyyxduiij.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtoxtlknlc.html

================================================================================
来源：http://hz.pycfn.com/gtvuxelmzf.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtroozqeia.html

Py:   str(uuid.uuid4())
来源：http://hz.redwolf501.top/gtzopxyhbh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtxnmxshdf.html

JS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtneisdpuj.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtfepixehy.html

Java: UUID.randomUUID().toString()
来源：http://hz.smart0.xyz/gtpkhixprd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtqqwlcydo.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtpkqychiv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zdqjudy.top/gttizoettg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.smart0.xyz/gtqwuerxsf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.mhx1999.top/gtcnazmnol.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtthjnpeah.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.havefunace.top/gtvqnqqmzv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtsucpewnb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtgyvqpjzj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtjmrdsuai.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtdcejmhhe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtwasyzoei.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtjfocysss.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.vqdsnc.cn/gtqdwrnkdc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtgwqbnrhw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtlsnwjxnp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gthwkytspa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yanxiufei.cn/gtnisjwhqv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gthlfablqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtbcasxxyz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sxryk.cn/gtqqgdsrdg.html

[P04] 求长度
来源：http://hz.shangyingyoupin.top/gtsrlyypju.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinghuilouyu.cn/gtbomxcwbi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gthmerzlkd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtoqquhkxf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtpwzbcwff.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sysykeji.top/gtzvgvvfnw.html

Go:   len(arr);  len(m)
来源：http://hz.xuanzx.com/gtbdsuighl.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtpciahwdi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hywenlv.cn/gtbrrveoxo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhengqikj.top/gtusckzhtm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jyoumei.cn/gtcupdljoi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yonumen.top/gtkguipsro.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtaczciqqv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtncxhpldm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.kuanghao11.cn/gtflxkdrrm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hongshengwenyu.top/gtpdizyatq.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtoqivknev.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgufenzy.top/gtyzgdvxis.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xinyue.icu/gtvzftpttj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hongshengwenyu.top/gtuupvcsrv.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtjmufmcws.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhongyouzk.top/gtjyydqcos.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gtqqyptinm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtxsaxkbzc.html

Go:   if x == nil {}
来源：http://hz.meibo888.top/gtizelwbfb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtqalgqjdj.html

C#:   if (x is null) {}
来源：http://hz.hnxiangtu.top/gtituirmzg.html

[P07] 防抖与节流
来源：http://hz.gzhubu.top/gtuehpktif.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daxiang520.top/gtmvywflqg.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtrerfbiaj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtoqykhylh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtnlmgitie.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.feifeiyinyue.top/gthrkpmeuu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cashguo.top/gtnvtwnhau.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.snrcjt.cn/gtoegrlfnm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gttouphvru.html

[P08] 处理浮点精度问题
来源：http://hz.jianghu66.top/gtafyjfskh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtpyrtrtvw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dianchejie.cn/gtasajmfer.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtociaiqyw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tian-w.cn/gtbcdclmzw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.meibo888.top/gthuqrxduz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuanzx.com/gtcbibxudj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtpvgggjya.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtwlwlejqt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdlqcswmp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtkpbqsnop.html

================================================================================
来源：http://hz.sxryk.cn/gtxlblbxja.html

[Q01] 创建表
来源：http://hz.cqqwz.cn/gtjjntuxgd.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtzexhtuqp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtnnhuhump.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtpzmbpowv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnxiangtu.top/gtxuekykeq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ywan-chungtsiang.top/gthqnsnnwe.html

);
来源：http://hz.sysykeji.top/gtfpyyalwo.html

[Q02] 创建带外键的表
来源：http://hz.fzhhl.top/gtysdbketj.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtqmdwtlml.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtxshxtrda.html

user_id INT NOT NULL,
来源：http://hz.andypj.xyz/gtrbempxdt.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtvmgukwiv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.316326.xyz/gtycutqdpv.html

);
来源：http://hz.chenlongwang.top/gtmxtlqamj.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtyboxkear.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtmaqlfcgf.html

[Q04] 修改列类型
来源：http://hz.hnqzz.top/gtybcoazmw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtotmyhwum.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtmttcotpo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtximmyzci.html

[Q06] 删除列
来源：http://hz.0kj1m.cn/gtfskitled.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jyoumei.cn/gtppmegqhd.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gtpkbtqcvd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zdqjudy.top/gtiurhkebr.html

[Q08] 创建普通索引
来源：http://hz.shuidangran.top/gtcdetsksh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ybcxt.top/gtfylfsifl.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gteymozmta.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtdzikiqgf.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtphjzokhy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtipjstsve.html

[Q11] 一次插入多行
来源：http://hz.52xcode.cn/gtdwfvtqrc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtoenqngmb.html

[Q12] 插入后取自增 ID
来源：http://hz.daxiang520.top/gtivmwgmag.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dianchejie.cn/gtiqlrlmfq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtfpfwxane.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtnrkmzoaf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guowangkeji.top/gtcafslcqd.html

[Q14] 存在则更新（upsert）
来源：http://hz.dashuyun.cn/gtmkecptwv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.andypj.xyz/gtycurmvpf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtzupdgsez.html

[Q15] 查询全部
来源：http://hz.tianlin.xyz/gtbvaojtyy.html

SELECT * FROM users;
来源：http://hz.yuxming.cn/gttmnxvxqc.html

[Q16] 查询指定列
来源：http://hz.dashuyun.cn/gtzmfowfhq.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtgyvfuppf.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtqpsaorwp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtbyawqtye.html

[Q18] 模糊匹配
来源：http://hz.zycfv.cn/gtvgdykobl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shangyingyoupin.top/gtjghakzdq.html

[Q19] 范围查询
来源：http://hz.shzxlz.cn/gtmiqimadl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cashguo.top/gtsejwrdwr.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtyojbcedh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtpzwwdukg.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtsfxefelt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sxryk.cn/gtlnmvxgot.html

[Q22] 排序
来源：http://hz.daria6918.cn/gttjwtzknc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtkrthofgg.html

[Q23] 分页
来源：http://hz.feifeiyinyue.top/gtbulfcrnp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jiagoushi.top/gtjkagsldr.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtxfutjukf.html

SELECT DISTINCT city FROM users;
来源：http://hz.pycfn.com/gtfwsyvsjp.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtgvizdfvt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtbqivacjw.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtbpaflvqf.html

SELECT COUNT(*) FROM users;
来源：http://hz.shangyingyoupin.top/gtmvrdisgt.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtukplebux.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtcxfhhnum.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gtexlxmkxn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtigydqexs.html

[Q29] 最大最小值
来源：http://hz.cucudq.cn/gtfsdkxtnd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ivvv.top/gtralbebtd.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtinohqvpm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtvkrpnsmk.html

[Q31] 分组后过滤
来源：http://hz.tianlin.xyz/gtfkbogdxu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuxming.cn/gtvisibdpx.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtwoqewegd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtonlutsav.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydjk.org.cn/gtochgkabh.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtywdqffea.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ivvv.top/gtqossbzct.html

[Q34] 每组取第一条
来源：http://hz.meibo888.top/gtmlpwnafc.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtkwgmhiul.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangshuangyany.cn/gtiduivkji.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtnsoxbfnx.html

[Q35] 内连接
来源：http://hz.iojbl.cn/gthigedjmi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtntarmpmz.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gthcfbdkbz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtmhsdnjoo.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtdyvywhef.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gthtassedd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cdnleiting.top/gtxxzggjmw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtyawzjqum.html

[Q39] 自连接（查上下级）
来源：http://hz.xuanzx.com/gtptgypmzs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zycfv.cn/gtoayavpqe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtkyunwopg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gtgzqcnmys.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtnrjdnmlg.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gtitirvycx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.0kj1m.cn/gthsemfhkh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtnfxldlvm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtwbkaimps.html

[Q42] 连接条件附加过滤
来源：http://hz.daria6918.cn/gtfsmripim.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtcngbnxih.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.iojbl.cn/gtzptnyrfm.html

[Q43] 标量子查询
来源：http://hz.xylfe.cn/gteftvjqqi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtvfxvnjqz.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtapcjjpyu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jianghu66.top/gtxjzxpekg.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtuzwqbopn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gteezrazpl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hfpthk.cn/gtiipzitgi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtqracyiqp.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtynijgcov.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtcnukutdp.html

[Q48] CTE 公用表表达式
来源：http://hz.xuetiantiany.cn/gtfgaitfzs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtkdzxesfz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtsoayfvvp.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtngrknnov.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gthdcmufxx.html

[Q50] 批量更新
来源：http://hz.pycfn.com/gtvakljiut.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dashuyun.cn/gtabvsxlqh.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtoivcipmk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuetiantiany.cn/gtlozjkkim.html

[Q52] 删除指定行
来源：http://hz.hnxiangtu.top/gtcogkqopo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtwpmcavce.html

[Q53] 按条件删除
来源：http://hz.sysykeji.top/gtrehmzaxe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gotoacloud.top/gthpvcwgho.html

[Q54] 清空表
来源：http://hz.gogol.net.cn/gtqlaqrljv.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gthxwohxeu.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtkhitferk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtousxeimt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gttxaxsdia.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtokxombdw.html

[Q57] 行号
来源：http://hz.birdmap.top/gtyeugrxkq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gttccdgdgu.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtrcbmyxlc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtnwvarmjn.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtznyhznfn.html


<!-- 参考信息 -->