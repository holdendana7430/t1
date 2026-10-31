代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ae.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nn.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dn.lnxyls.cn

TS:   // 同 JS
来源：http://tl.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://tn.szsharing.cn

Go:   go f()
来源：http://sd.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ex.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://bq.521024.cn

[O02] 使用线程池
来源：http://mr.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hi.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sh.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://na.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://en.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oj.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://or.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uu.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fa.newstarts.cn

[O03] 加锁保护共享数据
来源：http://jk.hahajie.cn

Py:   with lock: shared += 1
来源：http://gz.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ji.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fr.521024.cn

TS:   // 同 JS
来源：http://az.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://ez.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pc.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nx.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://qi.hahajie.cn

[O04] 定义异步函数并等待
来源：http://bs.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://iz.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dl.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://wf.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pb.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nw.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xb.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ud.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://fr.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://ns.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://sy.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ot.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://xz.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://fh.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ep.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://en.huanxung.cn

Ruby: threads.map(&:join)
来源：http://pd.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://av.bookmarksfly.cn

[O06] 使用进程池
来源：http://do.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ew.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bo.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://ql.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://jk.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tc.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tk.hnjuh.cn

Ruby: // fork 块
来源：http://dr.wgjwhj.cn

C#:   Parallel.For
来源：http://el.yuexingan06.cn

================================================================================
来源：http://tr.wgjwhj.cn

P. 常用工具函数
来源：http://fm.bookmarksfly.cn

================================================================================
来源：http://qn.shxzskj.cn

[P01] 生成 UUID
来源：http://ad.521024.cn

Py:   str(uuid.uuid4())
来源：http://ai.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vu.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ug.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://kx.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://la.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://lg.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://pi.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://nl.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://gn.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ot.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://td.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gk.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gg.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ni.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wp.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uu.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ow.szxytkj.cn

[P03] 生成短随机字符串
来源：http://nm.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aa.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ik.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tn.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zi.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aj.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ct.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vu.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://or.muxihuayi.cn

[P04] 求长度
来源：http://wc.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wx.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pf.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ng.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://so.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://so.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://iq.panjiajie.cn

Ruby: x.length;  x.size
来源：http://jt.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ld.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://fw.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tm.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nw.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xq.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gm.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://be.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dt.huixinmuqiang.cn

Ruby: a == b
来源：http://ud.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eq.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pj.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://en.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://hk.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zt.nszjky.cn

TS:   if (x == null) {}
来源：http://yu.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://id.colortex.cn

Go:   if x == nil {}
来源：http://ba.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qf.hahajie.cn

C#:   if (x is null) {}
来源：http://tg.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://cy.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ev.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ov.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pz.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yz.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gj.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jj.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oc.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://av.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://im.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pa.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dg.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ea.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eb.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ut.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cf.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://un.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hr.szsharing.cn

================================================================================
来源：http://yw.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://th.bookmarksfly.cn

================================================================================
来源：http://ee.lnxyls.cn

[Q01] 创建表
来源：http://or.chemitech.net.cn

CREATE TABLE users (
来源：http://fm.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hq.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://ec.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://rc.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://de.bookmarksfly.cn

);
来源：http://fo.asd995.cn

[Q02] 创建带外键的表
来源：http://qo.nicolike.cn

CREATE TABLE orders (
来源：http://dw.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ue.jctech888.com.cn

user_id INT NOT NULL,
来源：http://zg.nszjky.cn

amount DECIMAL(10, 2),
来源：http://zq.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qb.huixiangedu.cn

);
来源：http://do.asd995.cn

[Q03] 增加列
来源：http://jw.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ey.shxzskj.cn

[Q04] 修改列类型
来源：http://qx.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://an.wgjwhj.cn

[Q05] 重命名列
来源：http://gw.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aq.jianghongdianzi.cn

[Q06] 删除列
来源：http://uj.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ny.muxihuayi.cn

[Q07] 删除表
来源：http://tm.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://ck.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://ja.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ar.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://en.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dr.9csxet.cn

[Q10] 插入单行
来源：http://zx.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ju.shxzskj.cn

[Q11] 一次插入多行
来源：http://bq.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vq.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://rx.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mw.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vy.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://ds.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lz.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://go.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bi.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://al.haigaiapp.cn

[Q15] 查询全部
来源：http://qa.szxytkj.cn

SELECT * FROM users;
来源：http://qy.jctech888.com.cn

[Q16] 查询指定列
来源：http://jf.hnjuh.cn

SELECT id, name FROM users;
来源：http://jo.colortex.cn

[Q17] 条件查询
来源：http://qh.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lm.colortex.cn

[Q18] 模糊匹配
来源：http://ja.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://de.haigaiapp.cn

[Q19] 范围查询
来源：http://au.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://up.shxzskj.cn

[Q20] IN 列表
来源：http://pt.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pa.huixinmuqiang.cn

[Q21] 空值判断
来源：http://ow.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tu.colortex.cn

[Q22] 排序
来源：http://ia.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://th.521024.cn

[Q23] 分页
来源：http://hq.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mq.jctech888.com.cn

[Q24] 去重
来源：http://lr.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://eh.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://wn.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fk.shxzskj.cn

[Q26] 计数
来源：http://fo.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://de.9csxet.cn

[Q27] 条件计数
来源：http://dm.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kf.521024.cn

[Q28] 求和与平均
来源：http://hc.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://de.szsharing.cn

[Q29] 最大最小值
来源：http://vl.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jr.yuexingan06.cn

[Q30] 分组统计
来源：http://hw.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ba.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://mv.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lt.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://mt.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yv.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eg.yuexingan06.cn

[Q33] 多列分组
来源：http://sp.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://em.jctech888.com.cn

[Q34] 每组取第一条
来源：http://pl.shtwfgs.cn

SELECT * FROM (
来源：http://em.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gy.huanxung.cn

) t WHERE rn = 1;
来源：http://hn.haigaiapp.cn

[Q35] 内连接
来源：http://qh.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tl.muxihuayi.cn

[Q36] 左连接
来源：http://gd.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://od.newstarts.cn

[Q37] 右连接
来源：http://ob.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rz.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://do.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yn.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://vj.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vn.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vy.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tf.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sq.9csxet.cn

[Q41] 多表连接
来源：http://ky.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xf.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://fy.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://qt.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://nw.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://zq.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://me.asd995.cn

[Q43] 标量子查询
来源：http://jb.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fh.muxihuayi.cn

[Q44] IN 子查询
来源：http://hu.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rn.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://ve.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lp.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cq.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cr.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ld.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qg.521024.cn

[Q48] CTE 公用表表达式
来源：http://xx.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xp.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://mi.lnxyls.cn

[Q49] 更新单行
来源：http://nl.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mq.yuntaijiaju.cn

[Q50] 批量更新
来源：http://nq.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ss.shxzskj.cn

[Q51] 用子查询更新
来源：http://zq.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wp.chemitech.net.cn

[Q52] 删除指定行
来源：http://bi.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://vi.chemitech.net.cn

[Q53] 按条件删除
来源：http://vr.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mh.yuexingan06.cn

[Q54] 清空表
来源：http://nj.huanxung.cn

TRUNCATE TABLE logs;
来源：http://na.521024.cn

[Q55] 排名（并列占位）
来源：http://uz.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bd.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://yz.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uc.nicolike.cn

[Q57] 行号
来源：http://zw.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ox.shtwfgs.cn

[Q58] 累计求和
来源：http://ki.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zk.shtwfgs.cn

[Q59] 分组内累计
来源：http://jf.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://um.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://mh.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uh.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dd.9csxet.cn

[Q61] 移动平均
来源：http://gw.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kz.jianghongdianzi.cn

[Q62] 分组占比
来源：http://yl.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kj.bookmarksfly.cn

[Q63] 开启事务
来源：http://hk.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cq.521024.cn

[Q64] 提交事务
来源：http://zu.9csxet.cn

COMMIT;
来源：http://dc.asd995.cn

[Q65] 回滚事务
来源：http://cq.wgjwhj.cn

ROLLBACK;
来源：http://dg.huanxung.cn

[Q66] 行锁查询
来源：http://ah.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bp.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://qo.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qo.huixiangedu.cn

[Q68] 保存点
来源：http://vw.huanxung.cn

SAVEPOINT sp1;
来源：http://ad.gzmigu.cn

ROLLBACK TO sp1;
来源：http://hw.asd995.cn

[Q69] 查看执行计划
来源：http://uo.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ug.chemitech.net.cn

[Q70] 更新统计信息
来源：http://kf.colortex.cn

ANALYZE TABLE users;
来源：http://dj.521024.cn

[Q71] 查看建表语句
来源：http://rz.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vz.shxzukj.cn

[Q72] 查看索引
来源：http://wp.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://eg.bjjhwx.cn

[Q73] 查看表状态
来源：http://ti.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tz.shxzskj.cn

[Q74] 强制使用索引
来源：http://zl.bookmarksfly.cn


<!-- 参考信息 -->