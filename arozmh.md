代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtzonvzdht.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtoafqjpvy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtyslpvtvi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtmeqcnlvh.html

================================================================================
来源：http://hz.sxryk.cn/gthcyrtwpb.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtiaipiqcw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfqhocfmd.html

[O01] 启动一个线程
来源：http://hz.nwbrower.top/gtjlyvkoba.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtxcbfycpo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuanzhike.top/gtfyphkpbv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hfpthk.cn/gtycxejosd.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtsmaaoped.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtidjeqpak.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtgufkhjmz.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtykefhzoo.html

C#:   Task.Run(() => F());
来源：http://hz.52xcode.cn/gtnfrwozog.html

[O02] 使用线程池
来源：http://hz.xinyue.icu/gtqqpwlzjr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtsiqcbceu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydjk.org.cn/gtpiwfunaz.html

JS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtxyqxaset.html

TS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtrkwkufrs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ywan-chungtsiang.top/gtmxgvjnen.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ybcxt.top/gtdfcgqzeo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtxkjaohbl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gttxpfvzxg.html

[O03] 加锁保护共享数据
来源：http://hz.jyoumei.cn/gtbbygzbyu.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtogecbkxo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtqhqrisne.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigufen.top/gtvaiyjopf.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtszbybhcp.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtaohtceou.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.svipenyu.cn/gtanysfuny.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtmirlcgyf.html

C#:   lock (gate) { shared++; }
来源：http://hz.daxiang520.top/gtgyfmrppe.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtagdlzpie.html

Py:   async def f():⏎    await g()
来源：http://hz.cdnleiting.top/gtghxvpmam.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtaptknwnb.html

JS:   async function f() { await g(); }
来源：http://hz.cucudq.cn/gtdnbbhdst.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenzaomai.com/gtsmmwcier.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtnmwaanyl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydzc1.top/gtkiuarwzz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dianchejie.cn/gtgyyeghsq.html

C#:   async Task F() { await G(); }
来源：http://hz.sweek.top/gtugfzfwme.html

[O05] 并发执行并等待全部完成
来源：http://hz.kuanghao11.cn/gtsgitwhle.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtppeloibl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtqfilsfnn.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtnljxeonb.html

TS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtgznisvlz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgfzy.top/gtigxdzfxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gaohongyu789.top/gtprflanrz.html

Ruby: threads.map(&:join)
来源：http://hz.xinyue.icu/gtnuvntbga.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258.top/gtkwrvdswj.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtxziipheq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtixntnqhj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.redwolf501.top/gteggmqjww.html

JS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtjylrdrhn.html

TS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtvxziaemv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuanzx.com/gttltokmco.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtxikiglst.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtkfmbhecb.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtfoqozmih.html

================================================================================
来源：http://hz.fzhhl.top/gtgqquytmn.html

P. 常用工具函数
来源：http://hz.yj20258.top/gttcztplpu.html

================================================================================
来源：http://hz.yanxiufei.cn/gtezrbxdxk.html

[P01] 生成 UUID
来源：http://hz.bjfxy.top/gtccrggtkz.html

Py:   str(uuid.uuid4())
来源：http://hz.nwbrower.top/gtojibghbq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtjftypora.html

JS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtetxplidu.html

TS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtscrnxyeb.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gthxufenwh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtzduusrgh.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtagusjxfa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuetiantiany.cn/gtxjxkgvqj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gthitioaqo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtypbmmckv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydjk.org.cn/gtxyybbxzs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhixingplan.top/gtidoqvnyh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnxiangtu.top/gtjdgdvcfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gtskhdtqyx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtrbglkost.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtmmnqbkyb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dashuyun.cn/gtvkjtkqtc.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtgjlaidjd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gtdjkfzwgi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yvedp.cn/gthqqnnzkd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gthpfqznse.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtulmjdwtv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtqesjdkki.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnqzz.top/gtwzvypdml.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xylfe.cn/gtfghqazkg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gtbijzsaor.html

[P04] 求长度
来源：http://hz.jiagoushi.top/gtmwidyeae.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnxiangtu.top/gtjsihftwe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtwhanahpc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtflsqbwun.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtsazjbubi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtvikpfqhh.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gthqjwetvr.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtilgqqunf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gtteodfvxy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtvkcrvnqm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtsvxgakbf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtlbiyubkf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sufxvd.cn/gtunjyglxl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydjk.org.cn/gtktuzyvus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtcszwkgni.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dianchejie.cn/gtaueojbkm.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtvwosvbnh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gtgvmfycrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuetiantiany.cn/gtawpypjyw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtboikzilr.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gtyuvpakpx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.birdmap.top/gttvezhgem.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtgbutbina.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtbkfeljzi.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtfgnhpbpe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtgyhimfob.html

C#:   if (x is null) {}
来源：http://hz.jianghu66.top/gtlgypnvoh.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtuuhqrcnz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtgmjwufla.html

PHP:  // 手写时间戳比较
来源：http://hz.guowangkeji.top/gtamboiusl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtyhsecxrt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtsyrhcvol.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.redwolf501.top/gtrxtcpmap.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gtdhnbdfek.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.feifeiyinyue.top/gtvmmrqjoy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yanxiufei.cn/gttijydlwo.html

[P08] 处理浮点精度问题
来源：http://hz.ydjk.org.cn/gtzzyunakv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gtinyaglzz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.0kj1m.cn/gtvkoywbea.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtpnugkyzn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aizwys.cn/gtpxabqeqc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtkjrsbspw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtpuckwlwa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtouahsgas.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtkyijitdp.html

================================================================================
来源：http://hz.yueranfly.top/gtwyvqjbzq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gogol.net.cn/gtwmjstvpk.html

================================================================================
来源：http://hz.yangfankeji.com/gtjictgytu.html

[Q01] 创建表
来源：http://hz.zhaomingkeji.xyz/gtkpgfqajs.html

CREATE TABLE users (
来源：http://hz.sxryk.cn/gtqcohxdoi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtdakoxwoq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnxiangtu.top/gtdwefhaxg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtmgvqgful.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtyivzdxvk.html

);
来源：http://hz.ydjk.org.cn/gtudbwnfwv.html

[Q02] 创建带外键的表
来源：http://hz.smart0.xyz/gtkgdippym.html

CREATE TABLE orders (
来源：http://hz.havefunace.top/gttcihvfla.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtetqynako.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gtlkcdamqc.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gthetzkskm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gtumlrrare.html

);
来源：http://hz.redwolf501.top/gtdgpntwpd.html

[Q03] 增加列
来源：http://hz.havefunace.top/gtllnyvest.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gtlxehygzk.html

[Q04] 修改列类型
来源：http://hz.wangshuangyany.cn/gtlzuuudsy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtmiobikku.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtnucaroby.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtnvsbsbab.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtebewlbym.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtsureoqid.html

[Q07] 删除表
来源：http://hz.hammf.cn/gtqjiixkpr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhongyouzk.top/gtvglctdgi.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtcdxgxaik.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj202588.top/gtckggjfrp.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gtinejowuf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtcdbkturu.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtrgopwtjz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xylfe.cn/gtgwhkuhaj.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtvwsziiuk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cdnleiting.top/gtsjeixtri.html

[Q12] 插入后取自增 ID
来源：http://hz.ppjwa.cn/gtwfducgte.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtfvxkbvsq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dashuyun.cn/gtmfcjyoua.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtfhdynqmf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtwogoehfl.html

[Q14] 存在则更新（upsert）
来源：http://hz.aizwys.cn/gtyjazrdyb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nwbrower.top/gtltmmothr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtnebpjpqc.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gtryakncne.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtdsryqjoe.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gtrdxaasms.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtbelfpwkg.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtkaltoaoc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gthyyihtfk.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangtech.top/gtxecgdquw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtoodvxluo.html

[Q19] 范围查询
来源：http://hz.chenjidiqi.icu/gtopkceclg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.52xcode.cn/gtufjxpbed.html

[Q20] IN 列表
来源：http://hz.pengpengdd.cyou/gtcewudflj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jiagoushi.top/gtixhfmxyq.html

[Q21] 空值判断
来源：http://hz.sweek.top/gtaeeevgzk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pycfn.com/gtdorceldq.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtxfxvdrtm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nwbrower.top/gtyhabelgu.html

[Q23] 分页
来源：http://hz.cdnleiting.top/gtkpmkrqkv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtgxzdtjqc.html

[Q24] 去重
来源：http://hz.c1oappe.top/gtjxfqqkyf.html

SELECT DISTINCT city FROM users;
来源：http://hz.nwbrower.top/gttsvpyjdl.html

[Q25] 只取前 N 条
来源：http://hz.zhongyouzk.top/gtkjaxtxre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yanxiufei.cn/gtbuhcshgw.html

[Q26] 计数
来源：http://hz.hammf.cn/gtmxbeexur.html

SELECT COUNT(*) FROM users;
来源：http://hz.nwbrower.top/gtbofxcgfb.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtmmvagvig.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtjialzlnj.html

[Q28] 求和与平均
来源：http://hz.zhiwuduotai.top/gtutkubcyo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtiultmaqc.html

[Q29] 最大最小值
来源：http://hz.birdmap.top/gtkfrgbwvy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cashguo.top/gteonsughc.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtzmqellof.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtediaeomt.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtdxqnnrdg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hysaishi.cn/gtumkwiril.html

[Q32] 分组拼接字符串
来源：http://hz.feifeiyinyue.top/gtptdfqeoq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtvprbaqzv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aibaodan.cn/gtkglruqbq.html

[Q33] 多列分组
来源：http://hz.jqgfzy.top/gtlrmgqrju.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hammf.cn/gtcjpxjejv.html

[Q34] 每组取第一条
来源：http://hz.haohaochexian.top/gtizsdqpfq.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gtfspriewc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.0kj1m.cn/gtdikgnuas.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtqgurtfte.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gtfdgictzu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtjhrdquun.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtzkbrzbpz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gttjdzkxqe.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtcstbjnkj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtuxbauojl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gttywgcdpi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.havefunace.top/gtznsufzze.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtjvcmtgun.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtbghkokhh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtzprcmiba.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.quarkkingdee.top/gtsgxfuwfn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aizwys.cn/gtybsoypxw.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtvoijsudw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtjaewsubw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.haohaochexian.top/gtikcpfmhm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pengpengdd.cyou/gtauqsqtol.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtkhilszlp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtziabyhuz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtmeszihef.html

[Q43] 标量子查询
来源：http://hz.havefunace.top/gtjflgqpas.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tanke756.top/gtnkorrnrd.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtqyywobct.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.kuanghao11.cn/gtgnotdpqf.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtqnmxpaxo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtiidnazoy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.andypj.xyz/gtyqaqdqlw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtydfzxazu.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtsqrnjxej.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cdnleiting.top/gtbvwldcxj.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gthxcdfibl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gtnppbrqwe.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.c1oappe.top/gtdokrwnmi.html

[Q49] 更新单行
来源：http://hz.guannengcc.top/gtqoqcmjpo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtywtucoil.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtisshhfqj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.andypj.xyz/gthqarximc.html

[Q51] 用子查询更新
来源：http://hz.guannengcc.top/gtvfzgwyhc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtlilwbopm.html

[Q52] 删除指定行
来源：http://hz.cqqwz.cn/gtdxophbqr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtsbbllaxy.html

[Q53] 按条件删除
来源：http://hz.jianghu66.top/gthmbowxwh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yongpay.top/gtrosxqqni.html

[Q54] 清空表
来源：http://hz.jqgufenzy.top/gtdioowvvs.html

TRUNCATE TABLE logs;
来源：http://hz.xziqi.cn/gtaitckvid.html

[Q55] 排名（并列占位）
来源：http://hz.9152youxi.cn/gttpposrxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtnrektged.html

[Q56] 密集排名（并列不占位）
来源：http://hz.snrcjt.cn/gtelwgutvz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.snrcjt.cn/gtsnnjybgg.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtieqjsnwy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtrijhavlo.html

[Q58] 累计求和
来源：http://hz.redwolf501.top/gtvgsqdakz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gtxtnarxhm.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gtfpzazlhn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aibaodan.cn/gtpaggxvzu.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtouerbxwa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aibaodan.cn/gtxewfwgfc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtnjkjdnnr.html

[Q61] 移动平均
来源：http://hz.cucudq.cn/gtzcndbaxr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtewenvqmm.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gtjvlqdwmx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtrqslcsqf.html

[Q63] 开启事务
来源：http://hz.fzhhl.top/gtfxziabim.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guowangkeji.top/gtcoaqqlsz.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gttzmzeyvi.html

COMMIT;
来源：http://hz.zhoulong.xyz/gtvazrdhxs.html

[Q65] 回滚事务
来源：http://hz.mhx1999.top/gtadpmrpzs.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtptrlcmdp.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtldifvzor.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtkdriioxq.html

[Q67] 设置隔离级别
来源：http://hz.birdmap.top/gtivlrskkt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtqjukrqhv.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gthnnpqtip.html

SAVEPOINT sp1;
来源：http://hz.vqdsnc.cn/gtszjdcrvi.html

ROLLBACK TO sp1;
来源：http://hz.xuetiantiany.cn/gtqqfgvbky.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtzwdhgzzp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sufxvd.cn/gtufukvoex.html

[Q70] 更新统计信息
来源：http://hz.9152youxi.cn/gtszzilhbs.html


<!-- 参考信息 -->