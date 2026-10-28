代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ivvv.top/gtfikmopxc.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gttvbbsqpk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtojvhrane.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtwbivfztv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtubrlxzlz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtlnlnueje.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gttipacini.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtzzrfbwfc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinyuanbaomall.cn/gtudwwmtxi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtspkwfrvi.html

[N11] 二叉树中序遍历
来源：http://hz.hysaishi.cn/gtjldtwwft.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtorijtrij.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gtpaeriwlu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gteofldgcv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtlgvehawb.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gtublissme.html

Go:   // 手写递归
来源：http://hz.yueranfly.top/gtuisluqco.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gzhubu.top/gtrxhjgeyx.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gthftdkhzv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtwmibpvyn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.0kj1m.cn/gtotqeedja.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gtylburods.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtoaeoohzy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtomykyzig.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtargkpmmx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daria6918.cn/gtqtutyjei.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtrektsjov.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtszdeauno.html

================================================================================
来源：http://hz.yongpay.top/gtjrwkixvs.html

O. 并发与异步
来源：http://hz.sufxvd.cn/gtdecbxrbz.html

================================================================================
来源：http://hz.daria6918.cn/gtsrpjfupn.html

[O01] 启动一个线程
来源：http://hz.nwbrower.top/gtfiyiiqdo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtxdqblnqs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangtech.top/gttaytzkpq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtordahnhe.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtryaqxzgi.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtobqpsxfb.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtcmfnqrwz.html

Ruby: Thread.new { f }
来源：http://hz.shuidangran.top/gtvseqqlxd.html

C#:   Task.Run(() => F());
来源：http://hz.smart0.xyz/gtgymvdevm.html

[O02] 使用线程池
来源：http://hz.jinqigfzy.top/gtxfoluoed.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtbwqyutbt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtcwqrzsmz.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtkitqdprq.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtmjaaspls.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pengpengdd.cyou/gtiltpmycq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gotoacloud.top/gtcbfosllr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gtmydybbgl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gtqquoakdv.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtrlegoekc.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtlaogtblk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtwtdvilxk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtbipddfwr.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtireaydvw.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gttvqpihal.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtrsiuzbpl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtqnnosulk.html

C#:   lock (gate) { shared++; }
来源：http://hz.gogol.net.cn/gtnmebwxta.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtigkfabiq.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtnuktmylf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xylfe.cn/gtuzumsjya.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gthiszltbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ybcxt.top/gtutjyyhgi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtnqgmrbcg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sysykeji.top/gtwgmjollj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.smart0.xyz/gtxxhikviv.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtuuzjbhcb.html

[O05] 并发执行并等待全部完成
来源：http://hz.yangfankeji.com/gtyjefuvjp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtsmzlnigi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj202588.top/gtbcaslihs.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtgmflqxkv.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtfigcxgei.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtohmfnasc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtkvxxtgry.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtrzmvtvnz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gtbppgjxpn.html

[O06] 使用进程池
来源：http://hz.nwbrower.top/gttgerdkbt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydzc1.top/gtmxalsvdx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtuaynvcny.html

JS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtauuznoxv.html

TS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtswglelld.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dianchejie.cn/gtwcshxboh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtmgxrpdwp.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtcduvzuku.html

C#:   Parallel.For
来源：http://hz.hywenlv.cn/gtovjlnbsh.html

================================================================================
来源：http://hz.hfpthk.cn/gtvnwwvhgk.html

P. 常用工具函数
来源：http://hz.havefunace.top/gtgelfgzju.html

================================================================================
来源：http://hz.andypj.xyz/gtxkziwqkx.html

[P01] 生成 UUID
来源：http://hz.hammf.cn/gtbeamrmbo.html

Py:   str(uuid.uuid4())
来源：http://hz.nwbrower.top/gttrrotzei.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtkanhulnm.html

JS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtpjnfkzrj.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtuyrmfhmv.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtzgzayrlo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ehwqpu.com/gttqrblhkm.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtorrnbkod.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtottnqrmg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtaxhgzmeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangdashe.top/gtcbankask.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtahqdewfz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gtvugfsljh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtbbgycfup.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtoomwhtsb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtyvcrubkz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gtgdxjnktd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtvwmzcgqt.html

[P03] 生成短随机字符串
来源：http://hz.andypj.xyz/gtsjcmnkst.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtiwqdlseu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gtlfhnilvb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtyobnyklj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gttycxpmzg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydjk.org.cn/gtmwivoatu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtwobempcd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shzxlz.cn/gtyevlfzbc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhiwuduotai.top/gtzffupsrz.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtzxukkgbw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinyuanbaomall.cn/gtfohffjmz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtxnyqyadt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtnccrhcxu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtdmijdxte.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtmygxthzw.html

Go:   len(arr);  len(m)
来源：http://hz.daria6918.cn/gtlacaygsj.html

Ruby: x.length;  x.size
来源：http://hz.yuanzhike.top/gtofzkbbrn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtzvspdisu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gaohongyu789.top/gtpgipjihx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtcyczahbk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtwdlwfsmh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gotoacloud.top/gtgvtmhknn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtfczgfzvi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangtech.top/gtpgmvadwr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gtiaoawhqm.html

Ruby: a == b
来源：http://hz.cheryme.top/gtxbhqufbm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtjlhgxzdc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtmhpdfoof.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxuanxn.top/gtifvgeslp.html

PHP:  if (empty($x)) {}
来源：http://hz.meibo888.top/gtfupmbfos.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ivvv.top/gtakkwrfyb.html

TS:   if (x == null) {}
来源：http://hz.ywan-chungtsiang.top/gtsructjsm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtvmupayrt.html

Go:   if x == nil {}
来源：http://hz.52xcode.cn/gttjkxxpxo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yueranfly.top/gtqbyflqhz.html

C#:   if (x is null) {}
来源：http://hz.daxiang520.top/gtkpebzwso.html

[P07] 防抖与节流
来源：http://hz.yongpay.top/gtuplycfbh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gterlonzlb.html

PHP:  // 手写时间戳比较
来源：http://hz.zhoulong.xyz/gtobhavlpe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtadxwhjjt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtugwpcpwb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tianlin.xyz/gtjnajmcxg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtwknnssde.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtvifoplai.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtprpbbhaq.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gteyxnzpiw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtkkmsrxzq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gtjyycxzfp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhoulong.xyz/gtxnxgzutv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gttzdxzbag.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtlkaookyo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangdashe.top/gtclxmwbee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gterlmvhal.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.0kj1m.cn/gtmpftxdbz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtprtcnuwk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtdqczvnxc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtifkhygpw.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtclimxbbe.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtbbphdibw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtsgdazejx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuxming.cn/gtkuunezyk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtffknwggr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinghuilouyu.cn/gtkqvrsnzi.html

);
来源：http://hz.iojbl.cn/gtbqrsloie.html

[Q02] 创建带外键的表
来源：http://hz.xziqi.cn/gtwbelcifc.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gtbbnncvpl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtrnggqgwg.html

user_id INT NOT NULL,
来源：http://hz.gotoacloud.top/gtvfpolzxi.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtmdtictpx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtdvgipcfi.html

);
来源：http://hz.jinqigfzy.top/gtxxususby.html

[Q03] 增加列
来源：http://hz.cdnleiting.top/gtnrqrmmod.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tianlin.xyz/gtvcuiemzr.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gtwapijkye.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtgegqyefq.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtenjwyxjc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtqyhioozm.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtrfzyypms.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtvcvibixl.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gthaqzwpbt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yanxiufei.cn/gtasuqngaw.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtsozlajfl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtpztamqgl.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtrhdbdtwo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtiyaigokp.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtedzdfqvm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gtxxbwrntl.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtudtofsud.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zdqjudy.top/gtolxhpjii.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtbuiqfdcf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtcdmvgoth.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.52xcode.cn/gtxsswyphz.html

[Q13] 忽略重复插入
来源：http://hz.guowangkeji.top/gtlktiyczk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gttfvfepaz.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtobuqsirs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtljmwwfxb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aibaodan.cn/gtnviswiai.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtbmlgarkk.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtfjexmpti.html

[Q16] 查询指定列
来源：http://hz.cqqwz.cn/gtnnklochx.html

SELECT id, name FROM users;
来源：http://hz.guannengcc.top/gtwmsbjorg.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtxbklkrkt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hammf.cn/gtmrrntxoo.html

[Q18] 模糊匹配
来源：http://hz.yongpay.top/gtpvjbfiys.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtbrzkddwp.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gtvfpecsyc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.bjfxy.top/gtmmdymgtj.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtgiddqnda.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhengqikj.top/gtadyjbagl.html

[Q21] 空值判断
来源：http://hz.kuanghao11.cn/gtlzxhodtu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ybcxt.top/gtusexhqeh.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtgspapynt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenjidiqi.icu/gtjlsdocbn.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtwzrukjhg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtfysphokf.html

[Q24] 去重
来源：http://hz.yuanzhike.top/gtkfsaexzz.html

SELECT DISTINCT city FROM users;
来源：http://hz.ppjwa.cn/gtecoplmma.html

[Q25] 只取前 N 条
来源：http://hz.yvedp.cn/gtjrqstxbw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtnqneglgb.html

[Q26] 计数
来源：http://hz.sxryk.cn/gtqrisrpob.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtscknxtrv.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gtcnuolwvi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangshuangyany.cn/gtijgiksyy.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtzgbcfxsi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtrnhdaaou.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtuelwksnk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenlongwang.top/gtjhtevfjb.html

[Q30] 分组统计
来源：http://hz.xylfe.cn/gtzkddppjl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtihbdkxle.html

[Q31] 分组后过滤
来源：http://hz.zhengqikj.top/gtberprwzt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtjvtovwxt.html

[Q32] 分组拼接字符串
来源：http://hz.dianchejie.cn/gtqlxshypw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtjsxntwtw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hammf.cn/gtfzxymmrc.html

[Q33] 多列分组
来源：http://hz.chenjidiqi.icu/gtspbgabbp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ppjwa.cn/gtihcydcqz.html

[Q34] 每组取第一条
来源：http://hz.wangdashe.top/gtsydgbqhp.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gtinacznzc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtbvnkswkk.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gttdfzzjwl.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtvzahqkub.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtbvuytwvu.html

[Q36] 左连接
来源：http://hz.hywenlv.cn/gtqsyjqbll.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtuiixxuqc.html

[Q37] 右连接
来源：http://hz.chenzaomai.com/gtxoyfimtd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtdvhervph.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gtolvanrgj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hywenlv.cn/gtuzwlwrzr.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gtwicnwdxp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gtfjdamqgj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigufen.top/gthntachpl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtkifxltvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtovpcvprb.html

[Q41] 多表连接
来源：http://hz.0kj1m.cn/gtqnfitjxt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj202588.top/gtywbbdica.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtxcwcweiu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.havefunace.top/gtrwosxixk.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtdnkadlit.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinyuanbaomall.cn/gtgiwpvkvb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gzhubu.top/gtfmqashqd.html

[Q43] 标量子查询
来源：http://hz.zhixingplan.top/gtuyynahuv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtfbwuewtj.html

[Q44] IN 子查询
来源：http://hz.havefunace.top/gtcsrpayjl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtguzmdzjs.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtmfujsmff.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtmhjvaszz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhongyouzk.top/gtmbssdlno.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtpcoasklk.html

[Q47] 与平均值比较
来源：http://hz.jinqigfzy.top/gttjgeltfh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daria6918.cn/gtzrpjdhst.html

[Q48] CTE 公用表表达式
来源：http://hz.chenjidiqi.icu/gtdufaoume.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtqqfplxgn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuanzhike.top/gtonajludy.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtznugsvmm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hysaishi.cn/gtownhxfja.html

[Q50] 批量更新
来源：http://hz.sysykeji.top/gtmzdvzlfs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtkmldgmpv.html

[Q51] 用子查询更新
来源：http://hz.sufxvd.cn/gtmzwbetln.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yvedp.cn/gtfmigafaa.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtfculfkhs.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtdebcpnrk.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtbhkzzxwk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinyuanbaomall.cn/gtmuhceekk.html

[Q54] 清空表
来源：http://hz.xinyue.icu/gtnxiqnmdr.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gthayihmfu.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtcpvtrzbh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtlvprnpfa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tianlin.xyz/gtwymgnuei.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtxoaizujr.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtcymxadjp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cheryme.top/gtcnhwvqgk.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtqvairnpl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtoeyosrqx.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtikxzfjdj.html


<!-- 参考信息 -->