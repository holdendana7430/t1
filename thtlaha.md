代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kn.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://qa.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://wv.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://mj.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cl.lnxyls.cn

TS:   // 同 JS
来源：http://si.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://bt.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gq.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uh.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://ea.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://ey.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://pg.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lr.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://gb.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pn.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ef.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://no.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nf.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://rq.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://it.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://xm.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://az.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://bo.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://ve.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ua.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gn.hahajie.cn

Ruby: threads.map(&:join)
来源：http://fl.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dy.9csxet.cn

[O06] 使用进程池
来源：http://ti.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mz.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uq.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://vy.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://te.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vy.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vb.yuntaijiaju.cn

Ruby: // fork 块
来源：http://nx.jctech888.com.cn

C#:   Parallel.For
来源：http://xa.bjjhwx.cn

================================================================================
来源：http://hv.shxzskj.cn

P. 常用工具函数
来源：http://xi.asd995.cn

================================================================================
来源：http://gz.nszjky.cn

[P01] 生成 UUID
来源：http://xb.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://mz.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sr.521024.cn

JS:   crypto.randomUUID()
来源：http://cg.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://pf.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://fd.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://he.colortex.cn

Ruby: SecureRandom.uuid
来源：http://is.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://qh.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://lz.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gz.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ul.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yv.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mj.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ck.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lh.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://it.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yi.9csxet.cn

[P03] 生成短随机字符串
来源：http://bz.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hi.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bk.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zv.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ki.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eq.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kh.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mb.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zt.muxihuayi.cn

[P04] 求长度
来源：http://zl.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lc.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://he.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qn.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sg.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://nw.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://iq.panjiajie.cn

Ruby: x.length;  x.size
来源：http://qi.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ou.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://ki.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ae.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vz.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xc.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vr.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qe.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ri.colortex.cn

Ruby: a == b
来源：http://jb.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://re.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://he.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yq.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://yg.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zk.9csxet.cn

TS:   if (x == null) {}
来源：http://zc.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dh.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://pk.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://js.hnjuh.cn

C#:   if (x is null) {}
来源：http://zn.szsharing.cn

[P07] 防抖与节流
来源：http://yn.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hr.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://hk.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bb.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lk.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://at.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lx.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ud.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://lh.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xl.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gv.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bt.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ws.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ll.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nn.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fl.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jy.huixinmuqiang.cn

================================================================================
来源：http://iz.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://em.nszjky.cn

================================================================================
来源：http://el.hahajie.cn

[Q01] 创建表
来源：http://sp.hnjuh.cn

CREATE TABLE users (
来源：http://oz.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zg.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://kq.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://mq.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hh.bjjhwx.cn

);
来源：http://iw.gzmigu.cn

[Q02] 创建带外键的表
来源：http://xm.shtwfgs.cn

CREATE TABLE orders (
来源：http://hd.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ed.newstarts.cn

user_id INT NOT NULL,
来源：http://pn.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://ag.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tz.9csxet.cn

);
来源：http://tn.nszjky.cn

[Q03] 增加列
来源：http://yw.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://so.yuexingan06.cn

[Q04] 修改列类型
来源：http://ce.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qw.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ll.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bo.gzmigu.cn

[Q06] 删除列
来源：http://cx.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ka.yuntaijiaju.cn

[Q07] 删除表
来源：http://tz.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://je.shtwfgs.cn

[Q08] 创建普通索引
来源：http://at.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fx.asd995.cn

[Q09] 创建唯一索引
来源：http://bh.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rn.wgjwhj.cn

[Q10] 插入单行
来源：http://hp.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ip.szxytkj.cn

[Q11] 一次插入多行
来源：http://ii.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zn.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://uq.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pz.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://my.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://ri.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aw.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ee.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mc.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xe.wgjwhj.cn

[Q15] 查询全部
来源：http://wr.hahajie.cn

SELECT * FROM users;
来源：http://je.hnjuh.cn

[Q16] 查询指定列
来源：http://ad.nszjky.cn

SELECT id, name FROM users;
来源：http://ih.9csxet.cn

[Q17] 条件查询
来源：http://da.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ws.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://oe.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xr.hahajie.cn

[Q19] 范围查询
来源：http://hy.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jp.panjiajie.cn

[Q20] IN 列表
来源：http://za.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fy.colortex.cn

[Q21] 空值判断
来源：http://mw.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cf.haigaiapp.cn

[Q22] 排序
来源：http://iz.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gs.shtwfgs.cn

[Q23] 分页
来源：http://oj.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ik.bookmarksfly.cn

[Q24] 去重
来源：http://ih.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://jz.asd995.cn

[Q25] 只取前 N 条
来源：http://ij.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dx.haigaiapp.cn

[Q26] 计数
来源：http://ds.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://jh.newstarts.cn

[Q27] 条件计数
来源：http://vf.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://np.yuexingan06.cn

[Q28] 求和与平均
来源：http://ff.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fi.gzmigu.cn

[Q29] 最大最小值
来源：http://te.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sa.nszjky.cn

[Q30] 分组统计
来源：http://gb.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gl.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://fs.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uu.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://yn.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pf.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sq.shxzukj.cn

[Q33] 多列分组
来源：http://fa.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://du.gzmigu.cn

[Q34] 每组取第一条
来源：http://vr.hnjuh.cn

SELECT * FROM (
来源：http://hf.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cq.szxytkj.cn

) t WHERE rn = 1;
来源：http://wv.yuntaijiaju.cn

[Q35] 内连接
来源：http://ea.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vj.muxihuayi.cn

[Q36] 左连接
来源：http://oa.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cv.gzmigu.cn

[Q37] 右连接
来源：http://sp.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qw.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vi.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qv.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://rn.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zx.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kv.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://id.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xr.muxihuayi.cn

[Q41] 多表连接
来源：http://ds.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ex.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://do.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://et.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://vk.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://xg.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ek.9csxet.cn

[Q43] 标量子查询
来源：http://mq.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lf.bookmarksfly.cn

[Q44] IN 子查询
来源：http://ir.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jn.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://uy.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mv.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yz.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tg.shtwfgs.cn

[Q47] 与平均值比较
来源：http://ov.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ib.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://dz.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dt.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://gf.hahajie.cn

[Q49] 更新单行
来源：http://ea.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hj.521024.cn

[Q50] 批量更新
来源：http://xg.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cx.gzmigu.cn

[Q51] 用子查询更新
来源：http://jh.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ol.nszjky.cn

[Q52] 删除指定行
来源：http://vf.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://ku.asd995.cn

[Q53] 按条件删除
来源：http://la.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sb.muxihuayi.cn

[Q54] 清空表
来源：http://gh.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://mb.asd995.cn

[Q55] 排名（并列占位）
来源：http://ri.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bj.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://wp.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xm.newstarts.cn

[Q57] 行号
来源：http://pe.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wd.huanxung.cn

[Q58] 累计求和
来源：http://no.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kh.shxzskj.cn

[Q59] 分组内累计
来源：http://uf.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rc.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://jz.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://km.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ec.muxihuayi.cn

[Q61] 移动平均
来源：http://rx.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yu.bookmarksfly.cn

[Q62] 分组占比
来源：http://zr.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dj.shxzskj.cn

[Q63] 开启事务
来源：http://ps.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xc.huixiangedu.cn

[Q64] 提交事务
来源：http://yu.huixinmuqiang.cn

COMMIT;
来源：http://bf.bookmarksfly.cn

[Q65] 回滚事务
来源：http://th.huixinmuqiang.cn

ROLLBACK;
来源：http://tt.nszjky.cn

[Q66] 行锁查询
来源：http://vb.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ya.asd995.cn

[Q67] 设置隔离级别
来源：http://uh.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://as.huixiangedu.cn

[Q68] 保存点
来源：http://cw.gzmigu.cn

SAVEPOINT sp1;
来源：http://rs.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://jj.wgjwhj.cn

[Q69] 查看执行计划
来源：http://tq.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wv.521024.cn

[Q70] 更新统计信息
来源：http://pd.bjjhwx.cn

ANALYZE TABLE users;
来源：http://rw.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://of.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ka.huanxung.cn

[Q72] 查看索引
来源：http://cz.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://rb.nszjky.cn

[Q73] 查看表状态
来源：http://za.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://da.bjjhwx.cn

[Q74] 强制使用索引
来源：http://lf.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sw.bookmarksfly.cn

[Q75] 日期格式化
来源：http://da.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nd.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://am.colortex.cn

[Q76] 按天统计
来源：http://mr.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jf.haigaiapp.cn

[Q77] 时间加减
来源：http://bh.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gd.shxzskj.cn

[Q78] 当前时间
来源：http://ey.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nd.jctech888.com.cn

[Q79] 字符串拼接
来源：http://rx.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hahajie.cn

[Q80] 字符串截取
来源：http://oa.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://es.shxzukj.cn

[Q81] 字符串替换
来源：http://vr.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yp.haigaiapp.cn


<!-- 参考信息 -->