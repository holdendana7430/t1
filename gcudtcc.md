代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/goojcqqdo.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gqohplwjs.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gtpwrvkln.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gayaafele.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/guivcxscx.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gjdhqhure.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gqjsuwwfx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/ghvdinnom.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gorjfekns.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gnzuuiroe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcgwcszpv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/grdbqqapu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gkhsjcefc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gdsdozono.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gllrmtrbq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gxlqpjhst.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gnnsoegrv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gdmupgavx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhnfxwoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gulzucmhq.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gmrdleyog.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/ggcqqijqs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gzflgiysw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gcerbkbru.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gjhcjkqpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gngmlswnm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gqvtoause.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/ggtfcnage.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gewndpvep.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvsyobtcd.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/govrnjxyv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gotxexuvh.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gsdhovgqj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gmvnmxlzk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gjdauhvhj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gqjbuasjt.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/grkazjrxm.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gowuxpgtw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gazlzzuxv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gipqpsmug.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gdektzxqu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gjlfhwrvi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gyulezfgp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/ghabyyuet.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gjxxjnqem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/guotdjfrj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gzmwejzfy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gztefslzs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gbgfuxvsa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gtepzcwku.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqvihtuwy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gpesihdyx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gxgydrrpl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gkzdtagzz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/geistdeta.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/ghjvavyov.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gvnopyylr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gczzsfjis.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gvzdljsch.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gbelbpddz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/guwmvgjlr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvjmgqpnk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gqmvoiwmn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/guqqpqddo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gvtuwhleq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gyssvmwal.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gstrgbnzm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gtreoitlu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gjqyzxbcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gyvspewno.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gbfnygddw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gbqayzqqm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gegdpsmnd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gaxjjgnbf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grtkotfls.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gklcvdrzy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gpquyxrkj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/ggxhpevrs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/geuopwbzl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdvsrnd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gxvwsuszp.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gdosknwhu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghijadmuj.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gulcghizk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gfijbekqr.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gcqhyvhid.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gmpdgkbwt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gjpnqdcat.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gflmkztxy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gbpomvoxl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gzdstgrvb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gyojcexsp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gksrjiwin.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gyjdgcppj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/ghrvnraiw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gyauhkvqx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/grneuhiub.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/ggiuhoirh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gmedjiedk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gpuifqtfb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/goezdryqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gjpwcjdpo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gryxmoivj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gjjdzdgci.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gijlpqdyz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/grjrlstge.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gihvqurma.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gtvodlmcz.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gimvtlwuu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gvvojehev.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gmenyfoos.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/guppvlkys.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gyuntsuif.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gysqfzfeh.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gfhqnrwtz.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gjkrdzshb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbogftcep.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/guvtlnkqr.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gdusmfjrz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gtcrevhmo.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gjpkrkoaf.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gyzfxgwid.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gygpjizqv.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/ghlwtykkm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gprdbcrki.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gwcaanrtc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gmkwfaaes.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/geynrpggg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/garvugvtm.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gzxyjizib.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gwpfizoxu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gbenydxmv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gnmquwafk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gbyycqvsn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gblreotud.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gblthtoxa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gxalpmbof.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/ghjvwbxxr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnjbwlrnb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gnnsivklt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gvwpqwkpg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gozhoyint.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gzzjlnvka.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gcggxdepo.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gyymyujed.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gmryqgcqa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gadetqymg.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gwriqzztc.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/goqeulrve.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gexfqyvks.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grrodsfzn.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gddatcyfu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gpaknwhrs.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gbpkmixys.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gygsrbsbm.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gcmoqaeyp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gdbyzycdt.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gnueoodyi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggxyfxqng.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gnrogqzbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gaevhuofi.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gfjrdghhp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gnrctntat.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gbgtvndoq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gybrmgxgh.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/goncwvosg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gufpwyezv.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gklweycgo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/goipsgklk.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gwviihsnh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grypypfll.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/ghplznhvf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkyvfbkng.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gzudvaaot.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkucccjwo.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ghlierdbu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkvbojbxj.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gqmdgmnec.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gcidflzvd.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gvcauqbxg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gfufzizdj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/glwcpynoa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gsrpbzgvm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gpcrhrkvj.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gdiluvzwx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gzomoafbw.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gcdqodswu.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gtmofmhml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gjvyiqmik.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gmipbavme.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gaypnfkin.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmwcwcder.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/ghjevaesg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gsstglhxb.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gfcmhgchh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gtwsggund.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/goqjnfcqn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gowtntqel.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/ghebxaxaw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gdxjbhcay.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gbxpramhl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gqoeyxnrk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gwnbqdrwa.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gnktlimrb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gmmsdflvb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gpzbuolum.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gfeaodzrb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gjgyglmbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gxvdhjksj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/glsqmldrx.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gcumlozne.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gaifkgzag.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/glbmvwgwo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gtgjfvxwn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/ggesjvpdg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gwomfbdum.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gxoxnjgdu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gqtzcvtfr.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gbnhaeoyf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gfecwfhjb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/ghsgwzoxn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/greqqohim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gvbktmlub.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gleweqizw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnkqqglcc.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gzswyorpb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gendrppio.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gbnluwnsw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gixwiwwmd.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gezqioseh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ggdphpwpi.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gbvlyqnsg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gklviegtu.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gqmrfdhio.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gkfwertuq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gjskmbskh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gfaydlhss.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/ggyhjkkoc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gbpfcumfb.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gadhwxxhm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gusncyqja.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gfhzongfc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqoajboal.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ggsfnchsw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/geopmwuvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gcyobjiku.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gvkssxcrp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghslxjhmm.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gltjjtyei.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdkjxmijo.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gsestluuk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/glthibpym.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gahbtzhlw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gbjajnwaq.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gygarvriz.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gjlfmnwug.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/guuowzizi.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gqsuawpgt.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gwcpbtubz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gvxzkrvpy.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gcfforjqx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gzappnnyl.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/glvxkkixs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/glgaxxptx.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gtnkwwlss.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gelcsyzkb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gfonhsxpp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gurfejsgj.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gfjczknce.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gobajtuoy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gizmshaip.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gisgtqizj.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghtiyrlea.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gmqeuuqor.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gybxrgyzy.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gotlahlhn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/geypltazv.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gzgkkfpvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gozdqxkrk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gzdoksnaq.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gwoaopzij.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gvgzhwjmy.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/guxuofbfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gvbkmpiwg.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ghdltayvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gywogynkh.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gjhlqrwlg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gzpabtkix.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/ggvlrtdre.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gceicddwz.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gwhjphqjk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gomgdczck.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gccoqilwi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/genxnsbfh.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gddmayfuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gsjaczwlt.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gmaisgica.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwzqvmzem.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gflzrjhrh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gdupbfxoa.sHtML


<!-- 参考信息 -->