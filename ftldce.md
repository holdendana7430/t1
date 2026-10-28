代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtccktmfph.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtcbfunjbo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtjzxhzmgu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtgwdhzyyi.html

================================================================================
来源：http://hz.xziqi.cn/gtmdurgwww.html

O. 并发与异步
来源：http://hz.jqgfzy.top/gtjzlnbhww.html

================================================================================
来源：http://hz.dashuyun.cn/gtquruemob.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtfsvkayyy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtgtbwmkpr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yueranfly.top/gtqghxecxd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtyqmqykfu.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtlolsfchs.html

Java: new Thread(() -> f()).start()
来源：http://hz.shzxlz.cn/gtlshunmnd.html

Go:   go f()
来源：http://hz.ydjk.org.cn/gtmdqtfoos.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gtoxmllpkd.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtoyucvmka.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtnqnscyyi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhengqikj.top/gtzktkwjbw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ybcxt.top/gtmkaiakbl.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtacwxyuyz.html

TS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtjinoqgkl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtaidwmpwc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gtjdwlgwfz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gthbxpssma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.mhx1999.top/gtjryclsmc.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtpdogopkw.html

Py:   with lock: shared += 1
来源：http://hz.cashguo.top/gtnepmgqgh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtjmfavpec.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gtnfduabfx.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gthuotneyk.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtvscfouns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gtorxpoopb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.smart0.xyz/gtzwxktrzt.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtiokfohyk.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtnnukmriq.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtlmvcqrnf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtihmytspt.html

JS:   async function f() { await g(); }
来源：http://hz.zhoulong.xyz/gtjpzfrwat.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtmjbnbsge.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.meibo888.top/gtnsynttbn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtqxqxajuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangdashe.top/gtgtgbdpqs.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgufenzy.top/gtnkuzzwmt.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhixingplan.top/gtiomqtlfu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtxakiazia.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtukvvxafk.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtmwrajovw.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtcfnwkoti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cqqwz.cn/gtwoppppdo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ivvv.top/gtqkevdixv.html

Ruby: threads.map(&:join)
来源：http://hz.daria6918.cn/gtohqcdoto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxinkj.top/gttwwiqfgh.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtddcsunhh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.havefunace.top/gtaahzmlpa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.andypj.xyz/gtomolafoz.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtpexbrfct.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtooglzhki.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtzaolgztg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtuvqcknjp.html

Ruby: // fork 块
来源：http://hz.xziqi.cn/gtrlvwtrat.html

C#:   Parallel.For
来源：http://hz.yj20258.top/gtcyznjgwb.html

================================================================================
来源：http://hz.hysaishi.cn/gtekpapkob.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gteakolyik.html

================================================================================
来源：http://hz.sysykeji.top/gtemnkqptp.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gtwsgvmyok.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtfpsgkztr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gthknxpvkd.html

JS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtgsgovvyb.html

TS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtmuqzngbj.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gttypwzemq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gtgsstighg.html

Ruby: SecureRandom.uuid
来源：http://hz.ydjk.org.cn/gtwjrlkmcn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.c1oappe.top/gttthwevab.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtnufybuei.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ivvv.top/gtvbxffylf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hfpthk.cn/gtwvvznrra.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.316326.xyz/gtjfdmwbmo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtumlmgvjd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nwbrower.top/gtxhcsnxkj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ppjwa.cn/gtrwzhygna.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgufenzy.top/gtkgosimei.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sysykeji.top/gtgyrlpkuq.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gtsgttsjwi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hongshengwenyu.top/gtkqrlkjjn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gteszszerc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtiderxhdd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtgumelvuo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenjidiqi.icu/gtjuzjotru.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtnovsagzt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gttaxcajbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtvysksjzj.html

[P04] 求长度
来源：http://hz.yongpay.top/gtomskbroc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.mhx1999.top/gtrwqlawza.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtguaqogow.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtwhafqita.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtgaskussb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtpkjqwzpj.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtmyzktmxs.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gtkqrmmsir.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shuidangran.top/gtotsammyf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yanxiufei.cn/gtgidyhjfx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gtbzukqhxf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtrnsonsnh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shuidangran.top/gttkdlltgx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtkkujqzgm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuetiantiany.cn/gtieecoays.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangkeji.top/gtpzlvwscs.html

Ruby: a == b
来源：http://hz.nwbrower.top/gtdvdiunzi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenlongwang.top/gtahhnlsbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtuwexigsn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhixingplan.top/gtuspehfna.html

PHP:  if (empty($x)) {}
来源：http://hz.xylfe.cn/gtidhqltiy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtswaoeclw.html

TS:   if (x == null) {}
来源：http://hz.nanxuanxn.top/gtaqpodnnh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtwkbljcoz.html

Go:   if x == nil {}
来源：http://hz.jinqigfzy.top/gtlfzffqrg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhaomingkeji.xyz/gtnwucwelu.html

C#:   if (x is null) {}
来源：http://hz.shangyingyoupin.top/gtqqaphblq.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtkakmkcfw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gtqynjhhun.html

PHP:  // 手写时间戳比较
来源：http://hz.pycfn.com/gtjdnrrzeo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gthqeedndw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtwrgrtold.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtozlrnctd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtnabeyyil.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jianghu66.top/gtwkmzdqyi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yvedp.cn/gtqflrsygv.html

[P08] 处理浮点精度问题
来源：http://hz.zhixingplan.top/gtwjehgduw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cheryme.top/gtlenksjur.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sxryk.cn/gtskeqpanl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.52xcode.cn/gtcgjskmqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtitvrjyyn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gtwngzanvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cashguo.top/gtwnthmbhx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnqzz.top/gtlxjqhjgt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinqigfzy.top/gtnumygndq.html

================================================================================
来源：http://hz.snrcjt.cn/gtkasboheq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gtogxgmtpv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtojfdfizh.html

[Q01] 创建表
来源：http://hz.zhongyouzk.top/gthjldybff.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtqacxfljd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gthbcluylg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.c1oappe.top/gtohwxwjyu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtnghyvtkd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtxseswmjr.html

);
来源：http://hz.xylfe.cn/gtjdslefbg.html

[Q02] 创建带外键的表
来源：http://hz.jyoumei.cn/gttqfnsvqk.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtlrigumkw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtkbwlrwtn.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtwbofnnkk.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtedgtzvar.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xylfe.cn/gtjiiviosm.html

);
来源：http://hz.ivvv.top/gtlmmjnesp.html

[Q03] 增加列
来源：http://hz.yueranfly.top/gttofcaheh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guannengcc.top/gtdnzhhzgb.html

[Q04] 修改列类型
来源：http://hz.jyoumei.cn/gtqxxanwwp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtiebyvxvr.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gtmigxkxnx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jianghu66.top/gtavqmslre.html

[Q06] 删除列
来源：http://hz.hammf.cn/gtoyjvknxv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gtsasnlycm.html

[Q07] 删除表
来源：http://hz.pengpengdd.cyou/gtaxgvwonl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtxsvpakik.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtflajiswf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtcqoccqap.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtdaayatfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtqxbffxnf.html

[Q10] 插入单行
来源：http://hz.daxiang520.top/gtfiiypggr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangkeji.top/gtqdlexhaa.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtsftuzfgo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jianghu66.top/gthavrzste.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtaecezekp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jyoumei.cn/gtshmxdsqf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtudptzudn.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtsaucdjxg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dianchejie.cn/gtwezvzabn.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtipfspnzb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gttbpxgave.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gteivatmgg.html

[Q15] 查询全部
来源：http://hz.bjfxy.top/gtntdtcdmr.html

SELECT * FROM users;
来源：http://hz.mhx1999.top/gtlxwlkpcd.html

[Q16] 查询指定列
来源：http://hz.jianghu66.top/gtkyhkvefu.html

SELECT id, name FROM users;
来源：http://hz.hnqzz.top/gtdnqwqvlj.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtpjbrkrcr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gtklgpgwov.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtvtadparm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtkzrffjpo.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gttgqppwpq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtexegwqdf.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtjlukudhi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtbjuvjbxm.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtcctxklwh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtmrjenwuu.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtpbyfjvgo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gttuyugoyi.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtqhujcylt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.meibo888.top/gtdkwcxhlq.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtldicelle.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtfopwgddk.html

[Q25] 只取前 N 条
来源：http://hz.wangdashe.top/gtuljmlhkt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hongshengwenyu.top/gtuaxudavj.html

[Q26] 计数
来源：http://hz.cashguo.top/gtidprnpbo.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtmahbkstk.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gtryopasup.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtoydinosp.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtyazbatlz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.vqdsnc.cn/gtnuzkczbv.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gteajziqmq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gttizetavp.html

[Q30] 分组统计
来源：http://hz.svipenyu.cn/gttftotflg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtxhlrjffs.html

[Q31] 分组后过滤
来源：http://hz.bjfxy.top/gtaqxdpuuw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtvswiqnen.html

[Q32] 分组拼接字符串
来源：http://hz.mhx1999.top/gtqxbqvydb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtjcrepcea.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtnliziyxe.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtqfywxesm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zycfv.cn/gttdbgilqx.html

[Q34] 每组取第一条
来源：http://hz.hywenlv.cn/gttxverwmf.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtbjyrcqww.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtlcggtxgn.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtyqavwuzg.html

[Q35] 内连接
来源：http://hz.zhongyouzk.top/gtustsigjw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtkqlottpa.html

[Q36] 左连接
来源：http://hz.jlsjyb.cn/gtfcgoeyry.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtgbwaxnkb.html

[Q37] 右连接
来源：http://hz.jinqigufen.top/gtifcrsboc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuxming.cn/gtknhmiqey.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtsjloanaj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtmtegbqjt.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gtrttiaode.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhiwuduotai.top/gtbkchcvir.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtltlnigsw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daxiang520.top/gtecgraiam.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydzc1.top/gtrlvmcspw.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtshmyrhyz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtxqpgjwlr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.kuanghao11.cn/gtawbihglj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gttqknxzqg.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gtwnhivljx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.andypj.xyz/gtvomtxtjf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtkxgvybnj.html

[Q43] 标量子查询
来源：http://hz.cucudq.cn/gtugezlkzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.bjfxy.top/gtecjddnfb.html

[Q44] IN 子查询
来源：http://hz.yangfankeji.com/gthxujptrc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydjk.org.cn/gtalioceei.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtvkstiwiq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtdugliijf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.bjfxy.top/gtshbekutz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtjgkcqyln.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtkakkxluj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gttmsvxwra.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtwxcwebfz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtwhjmdqle.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gthpleipjd.html

[Q49] 更新单行
来源：http://hz.dashuyun.cn/gtxmfjeqcv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtagzplezz.html

[Q50] 批量更新
来源：http://hz.dianchejie.cn/gtoawyauaa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.quarkkingdee.top/gtyuodcicc.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtijmpccec.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtdziframn.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtwlsjkkkb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtdzwdxdrs.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtmglfbxxn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hfpthk.cn/gtzzksgthj.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtomszmdzt.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtmsfjshgy.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtvqyvjluj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.meibo888.top/gtalyzpbat.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gtcaewstbt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtdzsyqfuo.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtziuyaste.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtwjwegchb.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gtduizuazb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtyvgtfzfi.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtfrtbtbcl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtmupowcpd.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gthgskhbpu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daria6918.cn/gtgrnjyezg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtjlkwkqns.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gttghavzdb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtmempiwqh.html

[Q62] 分组占比
来源：http://hz.hnxiangtu.top/gtboulpnts.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtlqcykchh.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtscwezqnn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gtiqxedkby.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtmygocvvh.html

COMMIT;
来源：http://hz.yvedp.cn/gtvpsrezcd.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtigaznqop.html

ROLLBACK;
来源：http://hz.cashguo.top/gtcuzrreyz.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtekqnsalv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtdjustcvk.html

[Q67] 设置隔离级别
来源：http://hz.jinyuanbaomall.cn/gtlwrtiubx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zycfv.cn/gtledruxem.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gtepgndubx.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtxoxrueie.html

ROLLBACK TO sp1;
来源：http://hz.yj20258.top/gtgbuoykcr.html

[Q69] 查看执行计划
来源：http://hz.hammf.cn/gtqqtubpql.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtpwgbjhvv.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtmbhuhbez.html


<!-- 参考信息 -->