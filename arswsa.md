代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jyoumei.cn/gtwutkrjvi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hysaishi.cn/gtvatwbhpg.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtzrmpvlvd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxuanxn.top/gtaflbdscg.html

PHP:  // 手写递归函数
来源：http://hz.gaohongyu789.top/gtmawepwyn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtbususdtn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtyjeaioiu.html

Java: // 手写递归
来源：http://hz.birdmap.top/gtrhladzfn.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtfyiiiaul.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtabcsjfsv.html

C#:   // 手写递归
来源：http://hz.c1oappe.top/gtynurcuec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtyngryryu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtplasdjcw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtzgsyebib.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtzntmrtkx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtibwgcdqu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtspfkckbe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtfoyngvdu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.vqdsnc.cn/gtdnvebmuu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtfybkcjox.html

================================================================================
来源：http://hz.nanxuanxn.top/gtolcvmblj.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtjvizyaqy.html

================================================================================
来源：http://hz.cucudq.cn/gtdhrfxqre.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtkdtexoeq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtmndqfvlw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtddohhsiu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtlmnapxyk.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtfmxoybae.html

Java: new Thread(() -> f()).start()
来源：http://hz.iojbl.cn/gtaxtxacdl.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtmidcqohj.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtnkkclqkj.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtmtiulcaq.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtryprheab.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hammf.cn/gtemliznmr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtvtsmhfvi.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtbmsqvwmd.html

TS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtudaexbmd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gttwrnrjmz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuxming.cn/gtflxzufev.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtdcdrwkqk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.redwolf501.top/gtftrhywzt.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtvljhuvdb.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtdfpmfren.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydzc1.top/gtjyelsasi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtwkmvcyty.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtqjmsnkqw.html

Java: synchronized (this) { shared++; }
来源：http://hz.zdqjudy.top/gtrxlqtrmv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhijiandao.cn/gtsxcnqiei.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ywan-chungtsiang.top/gtuohsaxrk.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gttajtidvu.html

[O04] 定义异步函数并等待
来源：http://hz.meibo888.top/gtutjrqpiq.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtdxmhljaa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pengpengdd.cyou/gtoywoepoj.html

JS:   async function f() { await g(); }
来源：http://hz.jinqigufen.top/gtjwbyiamn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fzhhl.top/gtjwjihizw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtvwwodtkz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtjfacctue.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtaykvpsgr.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gteqlzluew.html

[O05] 并发执行并等待全部完成
来源：http://hz.daxiang520.top/gtdoqlgitu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtzwfgeilo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.smart0.xyz/gtdrlhmark.html

JS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtxjnolvju.html

TS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtyoodhlea.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtmczcsgyh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zycfv.cn/gtywfllmba.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtkfycimxk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtnwvulixl.html

[O06] 使用进程池
来源：http://hz.ywan-chungtsiang.top/gtmpanqmza.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydjk.org.cn/gtphpsynmt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtlkckrvjb.html

JS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtbcojqcrn.html

TS:   // child_process / cluster 模块
来源：http://hz.meibo888.top/gtsokwqurd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hywenlv.cn/gtuyywdelu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gtcgtrbtza.html

Ruby: // fork 块
来源：http://hz.dianchejie.cn/gtdptgteyv.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtfbwdmust.html

================================================================================
来源：http://hz.daxiang520.top/gtivygrsro.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtmujkstum.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthwcmrcwm.html

[P01] 生成 UUID
来源：http://hz.0kj1m.cn/gtjlwqebbz.html

Py:   str(uuid.uuid4())
来源：http://hz.wangshuangyany.cn/gtdkdrjvpm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cqqwz.cn/gtpwjvworg.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtcatizarw.html

TS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gthdgscvrq.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gttgccvawq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pengpengdd.cyou/gthkesdrya.html

Ruby: SecureRandom.uuid
来源：http://hz.havefunace.top/gtrbdcwwaa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gthtairojy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtdvtqrhxs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtegzcbjbd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hywenlv.cn/gtnhmosbyf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aizwys.cn/gtudsxlxyl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cheryme.top/gtohyqnfei.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gtpwyadmlh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xingfuxueyuan.xyz/gtepeatsab.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gtvjsutcpk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258888.top/gtfjvangnu.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtpmbqgqwu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtutdydbiu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtkddximpe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtzooyffih.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtamnylpmk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtmatuoqhj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cheryme.top/gtsecpsepw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gtnswgfdus.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ivvv.top/gthntoecgw.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtlhrnigwd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtmztohrfq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtnrppdxgq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtyddclbai.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtewgcmqpe.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtiaixlmge.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtqhzlrsuw.html

Ruby: x.length;  x.size
来源：http://hz.jinyuanbaomall.cn/gtgywvqpxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtbgjuacqe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cashguo.top/gtlaqepmss.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtujoxjdbg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhoulong.xyz/gtdegfeeje.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.smart0.xyz/gtzbowqmfb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtismiwjui.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtudwrxuld.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtiradjvvi.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtxhgwtbuy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtpovividt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shzxlz.cn/gtbzsuxsyi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xingfuxueyuan.xyz/gtalcpnthe.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258888.top/gtvmsvubjh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sufxvd.cn/gtchpnriqr.html

TS:   if (x == null) {}
来源：http://hz.meibo888.top/gtvjmjcqbi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtqsnwupzu.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtmggokrwv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gtykpoenvt.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtibxxdjga.html

[P07] 防抖与节流
来源：http://hz.quarkkingdee.top/gtiihathbq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtkldrdnzk.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtwyexasiv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtxdbocgxy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtyudwyjxu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yanxiufei.cn/gtprnlyvjb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtzsoepffj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtfpikfoyq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sweek.top/gtrxcftolf.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtuulbjyhc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.kuanghao11.cn/gtukikblri.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hywenlv.cn/gtajvfnjhx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gtrqmdbnuk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtgdktpamw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtcpscvpsd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cdnleiting.top/gtgxyjdsvq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ppjwa.cn/gtxcijbfmh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cqqwz.cn/gtjhboffxs.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlpxpzyaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gtgetcvexu.html

================================================================================
来源：http://hz.9152youxi.cn/gtteuatjzr.html

[Q01] 创建表
来源：http://hz.9152youxi.cn/gtxnxhzhfv.html

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtvpovjuzw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtpepqwhqq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.havefunace.top/gtzejuhpsk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtbeynroaj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.9152youxi.cn/gtqahhbemy.html

);
来源：http://hz.cashguo.top/gtknagluqe.html

[Q02] 创建带外键的表
来源：http://hz.cdnleiting.top/gtbmnmmlxw.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtdjdnbpkm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtkdetvuml.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gthuqwadpc.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtfkgxzckx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aizwys.cn/gtupuspupn.html

);
来源：http://hz.mhx1999.top/gttsllhahz.html

[Q03] 增加列
来源：http://hz.zhiwuduotai.top/gtxaqbbqdv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hfpthk.cn/gtvetiubqs.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtmrdxvzhv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtcumuradq.html

[Q05] 重命名列
来源：http://hz.birdmap.top/gttouckmjy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xylfe.cn/gtvvgzeqyv.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gtsojigpwo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hammf.cn/gtnogrytnn.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtcngxsiem.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gtykqykwkt.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtbaaciptm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtaettnota.html

[Q09] 创建唯一索引
来源：http://hz.yvedp.cn/gtexmweocd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtyhjupxat.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gtfpmpalxu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hysaishi.cn/gthyrshksn.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtehzkwuzi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cucudq.cn/gtnzfohdlk.html

[Q12] 插入后取自增 ID
来源：http://hz.haohaochexian.top/gtoyzcpmfp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhongyouzk.top/gtwyewnott.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hfpthk.cn/gtxqcnxtvr.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gttqjndilb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shzxlz.cn/gtznmhxuof.html

[Q14] 存在则更新（upsert）
来源：http://hz.cucudq.cn/gtfoarelgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gttzaaptwv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtiuljgfmx.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtpdlbufnh.html

SELECT * FROM users;
来源：http://hz.hysaishi.cn/gtqcetagea.html

[Q16] 查询指定列
来源：http://hz.cqqwz.cn/gtdjngzckd.html

SELECT id, name FROM users;
来源：http://hz.havefunace.top/gtwveocwws.html

[Q17] 条件查询
来源：http://hz.shanyushiyangtech.top/gtyussgpft.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gtkyweoxsf.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gtmoqehhyz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gtupfgubbp.html

[Q19] 范围查询
来源：http://hz.ehwqpu.com/gtvobnsqdu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtjdnfaebh.html

[Q20] IN 列表
来源：http://hz.pengpengdd.cyou/gtlsesyndp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtfitodxoc.html

[Q21] 空值判断
来源：http://hz.ppjwa.cn/gtzrbrdmkq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtvstplpej.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtclfdzppq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gttmikaylt.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtczkvxrrj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gthzndhqzi.html

[Q24] 去重
来源：http://hz.yanxiufei.cn/gtlsluqbvk.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtaysvxwuc.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtzzswirux.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtuyqmlxog.html

[Q26] 计数
来源：http://hz.iojbl.cn/gtphbozbxy.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gttsaambdf.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtuwzvlpmo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtgmyzpsgm.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gtudfixdbv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtenfumpoz.html

[Q29] 最大最小值
来源：http://hz.aibaodan.cn/gtyjnyshjx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yuanzhike.top/gtdzwrmczv.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtvjldngxm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtsmqllxou.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gtsgeimoxq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtlzqbigdg.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtnjhtlphn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtpfopweum.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtkkvzwsuq.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gtgfqplxgp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cashguo.top/gtllvsgjlz.html

[Q34] 每组取第一条
来源：http://hz.zhaomingkeji.xyz/gtcyfnjagz.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtmhmdsard.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yangfankeji.com/gtzstgksig.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtoutyfthi.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gtnfgwumoc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtrcbwrcph.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtpfbsmsyy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtxfamxvnx.html

[Q37] 右连接
来源：http://hz.haohaochexian.top/gtgpumwsza.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtbkeoevql.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhijiandao.cn/gtfjybzpek.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gtoxrhqvrr.html

[Q39] 自连接（查上下级）
来源：http://hz.guannengcc.top/gtihunxoqf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.snrcjt.cn/gtqeedkpey.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.9152youxi.cn/gtwhthjbbt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.birdmap.top/gtjkqoclel.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtpolrvtxb.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtkalxkaks.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aizwys.cn/gtdinxmmqb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtgycycnxi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gthtadfviw.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtvvvswbfl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xinyue.icu/gtkxxraoqn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tian-w.cn/gtrkatkzja.html

[Q43] 标量子查询
来源：http://hz.nanxuanxn.top/gtolidvmkr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtbbgztrle.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtxwslgptj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.9152youxi.cn/gtpvvdnarz.html

[Q45] EXISTS 判断存在
来源：http://hz.feifeiyinyue.top/gtpcfrsuyq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtmwdzwskv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtbjpizksn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtikdpegrb.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gthzpyoydw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangkeji.top/gtltxatbws.html

[Q48] CTE 公用表表达式
来源：http://hz.svipenyu.cn/gtdphbnqug.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnxiangtu.top/gtbhfoqnsh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhengqikj.top/gtxwvnyzmb.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtvogztzhj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zdqjudy.top/gtidllngor.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gtprsxwypv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtdnigiunt.html

[Q51] 用子查询更新
来源：http://hz.shzxlz.cn/gtxfxougmv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgfzy.top/gtoexzmlow.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gtejlnbyil.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gtmcxkirpr.html

[Q53] 按条件删除
来源：http://hz.chenjidiqi.icu/gtsvatbril.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hysaishi.cn/gtsgpgvtfe.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtapzcpmzl.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gtznseshdm.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtfbeqgjib.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.9152youxi.cn/gtclmoffpt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtuyqlkdtk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtrlulzhgc.html

[Q57] 行号
来源：http://hz.xuanzx.com/gtflyrevhj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtqolpnikp.html

[Q58] 累计求和
来源：http://hz.gogol.net.cn/gtpwlwxrdo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gtskzewcbz.html

[Q59] 分组内累计
来源：http://hz.zhijiandao.cn/gtsiiapopn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangdashe.top/gtokiuxwyd.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhijiandao.cn/gtoksydcvg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gthuuxkdnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nwbrower.top/gtjipdjgmi.html

[Q61] 移动平均
来源：http://hz.jianghu66.top/gtfjuhignr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtohrxqrta.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtqiiglmhx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gttoxlwlkd.html


<!-- 参考信息 -->