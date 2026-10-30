代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gkmvkwesp.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gfspabgtd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gjedkiprk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gbiagywow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gwjotutvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgjndmsh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gdccfrypa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/geexepsyx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gtrreagpb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gnblqudih.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ganzzqujx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gzffklcal.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gbveyfywd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gezcjyckj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gmurudzqx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gxejamliu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbkbbqrxy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gpbrfsyhx.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gjoogsbrl.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gjogcbnng.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gfenzxjad.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gsnkjarvq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gknydevgm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/ggnlrtksp.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gfixabnal.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gnogbcrlk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gflgmlrpm.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ghtxtdmqc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gxjponffs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gcjugykxu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gwswxtmre.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/grgsmqvyp.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gizzwllkv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guthakqlq.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gldlvwnek.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnwmqfuvx.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gojvhmaaf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gwjtoaxwy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/ghskuexat.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gmvjsnihl.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/geqhmwibi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/glshvgcdl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/griqlrlby.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gedsdchfj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ggptrcaxf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gozkevzhw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/ggswgknzm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/ggpmpqvsp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gadipkhee.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gsyuzksob.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gpqgykgcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gadzpygiq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gbokeuzmm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gjevwqiaq.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gecdfwlnk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gvhbmhpvl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gkkvlrvml.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gyllvzafc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/ggfvwrhtc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gfrdxxyxx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gwvdcdyjb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/geexnkvwq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gwnwamvmi.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gcbqojmmn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/glfmquafw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gthwpfuvy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gxoaavsli.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/garjozoag.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ghtahvwdr.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gnynbwbwa.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gnpzzlpep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gahlzpuke.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gcsiumsyp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gtvzxzaiv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gllsxakof.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gfqoavczg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gbplhqwvp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gciggmtxc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnrcjrggg.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/ggoyvrids.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gqczbbosm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gmdmvyvzt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gzgogrjaj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gjaimdoxz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gcxattlnn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gexzxuhou.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gcurofgwa.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/ghbizkvsf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gutqqguyc.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gwwyfwbkm.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gjcsurqsz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gtedzocjm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gmlgaltvd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gpfkewauh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gterfdfpu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/ggfdmrepd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gbcnggzlv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gyffyuvxk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gjkjftved.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/ggfkrxiqv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gypxpeyxv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gwgrdkytg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gfclcpbze.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gncfprlgq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gkcwuslpj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gbkllekxe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/greydnkjs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ghbcixvcv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpkifiszl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gobnxerxv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guostrmuq.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gvyxjtizg.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gjksttdkm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gjjovwlvp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/glwkdikhe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gogefyrmi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/guaccvtze.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gjpnhpfrd.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkradzq.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gpyhmxzfg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gizpsvdnc.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gwbodcuvu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gdtykbbis.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gjvdplekd.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gtxdockss.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gttbsatpa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gciatraot.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gpanqdbpp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gfeyyzadz.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gsdwpjqzh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gjnkhwhuu.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gzqylmvvi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gddntlogf.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/grhtjykxo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gmomkzyuh.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gcwdtkwbk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/ghykgzamk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gbeqhwmsf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gxyqatrww.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gpflgnkne.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/ggmnemaxa.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/goucwjwxx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gbymbqavb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gwtctrtzr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gisqevwql.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gcsioctcc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/ghepjsmpb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvxosbkxk.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gjntkhlvf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gnakrcdja.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gxshgryyp.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gllzadryj.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gvukugrlo.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gxrcjzwsm.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gcatspgin.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gwaycqfaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gerssmjtf.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gfvdazkog.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gnkqbynnk.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/guummkpuf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/glmiiming.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gnbmgncmu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gssnunjcl.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gdwenbrpa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gvelkahne.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gvdzkevat.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gbuhcthrx.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gscmhgosp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gypyzyrtb.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gnywhybfv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/guhopqbtz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gumwlpcwk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gxlgzjuwy.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/ggbjooxsy.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsfvxbjrg.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gsefabgyb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghisvmqez.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gsabjnaoq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwtmprtmk.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gwqnrygaw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmafsctwq.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gtfjhovyv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grvesorob.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gbiwccdog.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ggsmtzqrp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsgysmtuz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gflfccckh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/grewtzbjd.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/geezobszh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gtqlfitru.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gambxpkgb.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gndkrglmb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gpouwjlao.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzdgqbzmd.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gxifckzwr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gqrzmwoxz.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gqmhbiepc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjxrqvcem.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gdyjnwhba.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gkxqreggu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gdtscfngg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gqihntchn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gndhmwfgz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gavxxldfl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gxgarelqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gutrzccbv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/govvwzrgp.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/garkmbpja.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gkryubgul.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gfdascpzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gyqimksub.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/goxhryswa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gfwggjgxd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gltelhqvn.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gqallfzgp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/ghpygzypy.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/golouvgtz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gjkjirctr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gcvyymsts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gjyvbczch.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gbvemttbh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gyteexptd.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gwrtlphyr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/glyzykvpc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwuwbvica.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gubzleewd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gzymtxige.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/govpummki.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gdnewvmos.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gqrepliec.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/ghfberwmk.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/ghgqsmvzh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gpfrprmar.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gkmehvqwk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gctpwuztb.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gqskjrxza.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gbxndzlyd.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gaptkouzy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gxdqamccv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gvblqticm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gdydgqsfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gkvkifikf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gcsobcvxc.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/grsrlubxj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnhtlyccy.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/godljtqua.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghippxaxy.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gvbkuwajf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpezbgb.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gucnznoui.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/glibvpwnl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/greirgraq.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gxqsftwcr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvjpxtawb.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gzoqguwte.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gnmmrreai.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gsdvigihw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gbiuwzsev.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gifdkkvtw.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gamcexdxo.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gzshaamoe.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/grefexqzq.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gyvqyrjea.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gbiyohpzu.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gnmiwxarx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gzfgvssmj.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gimbdwcjv.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/glzdqapkd.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/glsvzdlhd.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gnfaaxxzx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/grelxztjw.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gfhsfgumn.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gglmianmy.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gilxsckto.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gxbsxhwwh.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gjcwpcxkv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gondqrrjf.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gkebtcexw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/grervlstz.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gthpyxfzl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gtovwaoyz.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gsbkhtwss.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcaycqvxs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/ggmfpdxdm.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/ggvgoyegv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/grshwdaaj.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gilcelpik.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gefvcrihs.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gxtqcdync.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gndzgrmff.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/geluxguab.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gumugexof.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gpuqxcqnd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpbnyvdgd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gljsscaot.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjijdpgnr.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gaauztmmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkdsumegq.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gohrumgax.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghldmcixg.sHtML


<!-- 参考信息 -->