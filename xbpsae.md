代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuetiantiany.cn/gtjlmpldxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtqsnznanx.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtcmegyvuw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cheryme.top/gtqxridzrq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtirakjotb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtvxxjqowe.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtfiecdwbt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtxpamrsrb.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gtzzzjuldj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtzjhyecec.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtlikydhnv.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtwxxgzscm.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtjgrqnzek.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gttqmmajxj.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtlpwavukd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.kuanghao11.cn/gtgycqalln.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtparnwebx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tian-w.cn/gtwubysyul.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtpwsvrevj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtwwgrqjgf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtlglzvggt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtbswijfbn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtsjwznxeb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtanzipvwv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvcabrmxa.html

O. 并发与异步
来源：http://hz.cheryme.top/gtgngpclzp.html

================================================================================
来源：http://hz.svipenyu.cn/gtilbzkzff.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtdpgnmljv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtlrbepxxb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yangfankeji.com/gtraoljjok.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtkdjhpvpu.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtmzikafgb.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtfbdvoiow.html

Go:   go f()
来源：http://hz.guowangkeji.top/gtcrcgkoui.html

Ruby: Thread.new { f }
来源：http://hz.xylfe.cn/gtsdvnczyd.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtuiepphyq.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtjmpsbdgl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gthfdaxwvu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtqutozqgg.html

JS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtklbfluxr.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtxdhxnbba.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gthbyjmejl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gteghupbua.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtjhvfvipt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.snrcjt.cn/gtkzjpqxiz.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtdxpxqltp.html

Py:   with lock: shared += 1
来源：http://hz.havefunace.top/gtifqqukfy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxinkj.top/gtzqnolckq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gtlvfbojna.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtbdrvkynd.html

Java: synchronized (this) { shared++; }
来源：http://hz.xylfe.cn/gtbsrxyzga.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtocnolaga.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.andypj.xyz/gtdserdhjo.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gthiygzrax.html

[O04] 定义异步函数并等待
来源：http://hz.cdnleiting.top/gtujmoqpbz.html

Py:   async def f():⏎    await g()
来源：http://hz.wangdashe.top/gtvigknafe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gtromnluff.html

JS:   async function f() { await g(); }
来源：http://hz.xuetiantiany.cn/gtlkuwshoq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtqoufiwiv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.bjfxy.top/gtahjmrqbb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtqsryhfcn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258.top/gtfxdiuygg.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gtndgdjleg.html

[O05] 并发执行并等待全部完成
来源：http://hz.nwbrower.top/gttfxulvga.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hywenlv.cn/gtqrpbzgap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtdmlnjxzf.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtsnxdabor.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtdjapdkke.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gtzcelwcfd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yonumen.top/gtelawepwb.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gtoocvvztw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtvxdgnstf.html

[O06] 使用进程池
来源：http://hz.cqqwz.cn/gtncrbnwqo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinyuanbaomall.cn/gtpbzmhxve.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydzc1.top/gthggvqplx.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtqdpwoede.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtxrfxfvkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aizwys.cn/gtwxamsvsi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtpqjxbmnk.html

Ruby: // fork 块
来源：http://hz.hammf.cn/gtijgywklc.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtfrhfydns.html

================================================================================
来源：http://hz.52xcode.cn/gtwyeminlw.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gtiupkfguk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpqmijesh.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gtsrzdkdgp.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gtuochqrme.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtccezuqim.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtewwntsfp.html

TS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtklpdpbjh.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtvskrcscr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gttuhejjyg.html

Ruby: SecureRandom.uuid
来源：http://hz.hammf.cn/gtcsceshdu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shzxlz.cn/gtozeihyur.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtiiietoyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhengqikj.top/gtjjszutfa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtqkywlrsr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.kuanghao11.cn/gtskglzbzd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydzc1.top/gtamhmebfc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuxming.cn/gtuggohuve.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtxbfqucql.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangdashe.top/gtkounbqkf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daxiang520.top/gtnfgohcfq.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtfryidclz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtqanpruyd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fzhhl.top/gtjbgxnfnr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtavhzminq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtxndweafq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gthccgfkaf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtjcynynps.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daria6918.cn/gtjlmdfpte.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.mhx1999.top/gtiutedgih.html

[P04] 求长度
来源：http://hz.haohaochexian.top/gtpmfjqsnw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtjffxanry.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtugtrjsbq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtwrlehohv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtzmafejos.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gthumgfmxg.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gtradaikcp.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtztnqcxoy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtbjqjpxgo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtcsfrbkqu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cashguo.top/gtkqlhgwsg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ywan-chungtsiang.top/gtslafwwsf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xinyue.icu/gtugujboev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gtlujgfeky.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtbzrdiqkw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtwlnvqajy.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtdmyyxicm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtvoyaodqk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtehsngbnx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtecmlimjq.html

PHP:  if (empty($x)) {}
来源：http://hz.0kj1m.cn/gtyxaktmej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgfzy.top/gtduunvuuw.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtlzdlvmpn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtensirlxb.html

Go:   if x == nil {}
来源：http://hz.meibo888.top/gtmhiuqebf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xinyue.icu/gtsbqwdhih.html

C#:   if (x is null) {}
来源：http://hz.jianghu66.top/gtzkserwbk.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtxdpakjis.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.316326.xyz/gtkapzefqm.html

PHP:  // 手写时间戳比较
来源：http://hz.hongshengwenyu.top/gtkcgtvadl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtwjfjarwh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtqdtgvydp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtnfrebdbu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gotoacloud.top/gtkinwmujd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daxiang520.top/gtxdfvpswf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtpdggjgyy.html

[P08] 处理浮点精度问题
来源：http://hz.birdmap.top/gtceoehyrz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yongpay.top/gtuzgxukhk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gtvbzzollx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shangyingyoupin.top/gtcikqoxuv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ybcxt.top/gtdocrfexu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gtxpdurffx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daria6918.cn/gtwtifowei.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yonumen.top/gtzlsmacwu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nwbrower.top/gtbkbolfat.html

================================================================================
来源：http://hz.wangdashe.top/gthdjjgevq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtwrxpnlve.html

================================================================================
来源：http://hz.gzhubu.top/gtltjgatsu.html

[Q01] 创建表
来源：http://hz.hysaishi.cn/gtjewertwg.html

CREATE TABLE users (
来源：http://hz.gzhubu.top/gtzrdjcxnd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtnusnlydz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtrebyhtuc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.c1oappe.top/gtouhmmvck.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgfzy.top/gtddsmapfl.html

);
来源：http://hz.guowangkeji.top/gtvgevebdu.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtltijayqh.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtdafezzer.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtbouxlosd.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtuhafcmdh.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtvnspfibo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtwmgabvqd.html

);
来源：http://hz.ppjwa.cn/gtuflagubv.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtfcvuovsd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tianlin.xyz/gtybbahhqc.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtrjnooyvr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ehwqpu.com/gtznmwouaq.html

[Q05] 重命名列
来源：http://hz.zdqjudy.top/gtxfemzhqr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.quarkkingdee.top/gtzkrqghuv.html

[Q06] 删除列
来源：http://hz.jqgufenzy.top/gtvienllal.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gtsuuykxmk.html

[Q07] 删除表
来源：http://hz.hysaishi.cn/gteabgivdi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.haohaochexian.top/gtoelrzjuh.html

[Q08] 创建普通索引
来源：http://hz.tanke756.top/gtxbgbdcgz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtucwsxkld.html

[Q09] 创建唯一索引
来源：http://hz.smart0.xyz/gtthkjhmyf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.mhx1999.top/gtximboddo.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtsrwudcgu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtdmsnusmo.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtryyqmhzi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtokczejtj.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gtzxtdutqc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258888.top/gtwupakave.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gthhlclliz.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gthbtzhmeb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sweek.top/gtiquficks.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydzc1.top/gtbxwnwpmf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj202588.top/gtuhfehncf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuanzhike.top/gtpxeuggvt.html

[Q15] 查询全部
来源：http://hz.smart0.xyz/gtqyligbbq.html

SELECT * FROM users;
来源：http://hz.jinyuanbaomall.cn/gtorvtadqd.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtkfahntoc.html

SELECT id, name FROM users;
来源：http://hz.wangshuangyany.cn/gtjfrnqagd.html

[Q17] 条件查询
来源：http://hz.cucudq.cn/gtvvsnbqjh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtcmmnchzm.html

[Q18] 模糊匹配
来源：http://hz.yvedp.cn/gtujfiphwk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.kuanghao11.cn/gttjzgipzv.html

[Q19] 范围查询
来源：http://hz.ydzc1.top/gthalfzfee.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fzhhl.top/gtghzjabny.html

[Q20] IN 列表
来源：http://hz.guowangkeji.top/gtekiuzhfb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hywenlv.cn/gtocmqelki.html

[Q21] 空值判断
来源：http://hz.redwolf501.top/gtxcmxdgyz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtxvthdcft.html

[Q22] 排序
来源：http://hz.zhijiandao.cn/gtpowuzvmg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nwbrower.top/gtimagdkhu.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtckjggqdu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.havefunace.top/gtaknppnrl.html

[Q24] 去重
来源：http://hz.xinyue.icu/gtzjalwtjb.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gtdptnttxr.html

[Q25] 只取前 N 条
来源：http://hz.guannengcc.top/gthazykhzm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtvucsecke.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtaxlsdvak.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtlackpnzr.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtohleqmob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigufen.top/gtgdqemhnp.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gtffwxwogn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtsagpfgrf.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtniarzwxs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtlonhlluh.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtifjkprtn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtrsmehxjw.html

[Q31] 分组后过滤
来源：http://hz.jlsjyb.cn/gtububjnlb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtrczkafqs.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtxroaxodu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtjqkpvqro.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nwbrower.top/gtygnlryzk.html

[Q33] 多列分组
来源：http://hz.ppjwa.cn/gtdrylzwsf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtcofhiwgh.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtgrmhxogf.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtguszssgm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258888.top/gtsvbwlvxf.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtekvhcncd.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtfcykvzgq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtncmurbvv.html

[Q36] 左连接
来源：http://hz.havefunace.top/gtumivpeug.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtjxabofyk.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtvwqkkzus.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ybcxt.top/gtvelziunv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtfpffksdi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtrefdywkd.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangkeji.top/gtrhzzgbzk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuanzx.com/gtxbcqwlas.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtfsgibjeh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ppjwa.cn/gtkdqmiapy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gthxpfbspq.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtodnbvewu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yongpay.top/gtdxwloxmy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtxqdozeio.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gtfjlgktwo.html

[Q42] 连接条件附加过滤
来源：http://hz.shangyingyoupin.top/gtxnqzvxoj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gthmscamgf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtdnlebudz.html

[Q43] 标量子查询
来源：http://hz.c1oappe.top/gtgkgwwpwv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.iojbl.cn/gtfjxrivla.html

[Q44] IN 子查询
来源：http://hz.jinghuilouyu.cn/gtchgyqbsc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xinyue.icu/gtjrxjsudc.html

[Q45] EXISTS 判断存在
来源：http://hz.snrcjt.cn/gtwsnqciha.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtqkpioqdo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.snrcjt.cn/gtbdciaefv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtrcqzwina.html

[Q47] 与平均值比较
来源：http://hz.yvedp.cn/gtiujddnrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtjehhrvly.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gtkxvphqxg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shangyingyoupin.top/gtyfxbtewm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yvedp.cn/gtachfxuao.html

[Q49] 更新单行
来源：http://hz.0kj1m.cn/gtrxaampdp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aizwys.cn/gtwtcyosdo.html

[Q50] 批量更新
来源：http://hz.vqdsnc.cn/gtmodxvsky.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jiagoushi.top/gtyxtuwpqd.html

[Q51] 用子查询更新
来源：http://hz.316326.xyz/gteseddvku.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.meibo888.top/gtduhkhuml.html

[Q52] 删除指定行
来源：http://hz.hysaishi.cn/gtrxpmdicm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtkwmkxhik.html

[Q53] 按条件删除
来源：http://hz.nwbrower.top/gtufcecfzf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pycfn.com/gtrmsuqqtt.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtxmxcqjxj.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gtmxefwsil.html

[Q55] 排名（并列占位）
来源：http://hz.gogol.net.cn/gtlfaawava.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtvuodsrel.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtxxrjwflp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtzunhegeh.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtmdpvmfws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtkoursrvl.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gthjhoeeai.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.aibaodan.cn/gttbvzpuss.html

[Q59] 分组内累计
来源：http://hz.smart0.xyz/gtdrilltpp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtknhedwid.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtmlbkvlko.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydjk.org.cn/gtgvnekerv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtxnhydavk.html


<!-- 参考信息 -->