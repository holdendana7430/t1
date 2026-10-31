代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sn.chemitech.net.cn

TS:   // 同 JS
来源：http://wd.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://sm.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sr.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://et.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://gd.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://oh.asd995.cn

Py:   async def f():⏎    await g()
来源：http://py.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://so.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://te.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vh.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kj.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nw.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kb.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://sq.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://th.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://sz.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ux.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://ay.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://ov.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gp.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://we.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://pr.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nf.wgjwhj.cn

[O06] 使用进程池
来源：http://at.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mp.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jc.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://mc.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://cy.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ro.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ce.lnxyls.cn

Ruby: // fork 块
来源：http://sl.nszjky.cn

C#:   Parallel.For
来源：http://iz.haigaiapp.cn

================================================================================
来源：http://bl.hnjuh.cn

P. 常用工具函数
来源：http://bj.huanxung.cn

================================================================================
来源：http://ks.szsharing.cn

[P01] 生成 UUID
来源：http://al.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://by.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://co.newstarts.cn

JS:   crypto.randomUUID()
来源：http://fa.hahajie.cn

TS:   crypto.randomUUID()
来源：http://yh.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://br.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://tb.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://ri.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://pt.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ig.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pe.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qb.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kb.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lg.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aa.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ga.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yq.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yu.521024.cn

[P03] 生成短随机字符串
来源：http://vy.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://us.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ah.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bh.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ah.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sj.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ew.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kn.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wj.newstarts.cn

[P04] 求长度
来源：http://il.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ll.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sb.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gq.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xs.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://wq.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://wi.shxzukj.cn

Ruby: x.length;  x.size
来源：http://rb.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zs.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://iw.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wq.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jn.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ob.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jd.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ys.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oq.yuntaijiaju.cn

Ruby: a == b
来源：http://vt.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vw.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lq.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iv.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://vx.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ai.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://vf.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jx.huanxung.cn

Go:   if x == nil {}
来源：http://fk.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vb.jctech888.com.cn

C#:   if (x is null) {}
来源：http://ps.wgjwhj.cn

[P07] 防抖与节流
来源：http://kl.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xw.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://os.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oc.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zk.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mb.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zz.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vo.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uu.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://to.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ne.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yc.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mu.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uk.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rz.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ne.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xw.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uq.yuntaijiaju.cn

================================================================================
来源：http://hq.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yr.lnxyls.cn

================================================================================
来源：http://ea.newstarts.cn

[Q01] 创建表
来源：http://bf.huixiangedu.cn

CREATE TABLE users (
来源：http://co.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fg.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ec.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://rj.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bm.shxzskj.cn

);
来源：http://qt.asd995.cn

[Q02] 创建带外键的表
来源：http://py.nicolike.cn

CREATE TABLE orders (
来源：http://ed.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wq.shxzskj.cn

user_id INT NOT NULL,
来源：http://jh.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://jk.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iz.shxzukj.cn

);
来源：http://ho.hahajie.cn

[Q03] 增加列
来源：http://ri.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mc.muxihuayi.cn

[Q04] 修改列类型
来源：http://bb.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oo.huixiangedu.cn

[Q05] 重命名列
来源：http://ew.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://id.9csxet.cn

[Q06] 删除列
来源：http://wa.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ja.lnxyls.cn

[Q07] 删除表
来源：http://vc.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://mz.shxzukj.cn

[Q08] 创建普通索引
来源：http://uo.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wz.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://th.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qm.newstarts.cn

[Q10] 插入单行
来源：http://xr.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mz.szxytkj.cn

[Q11] 一次插入多行
来源：http://uv.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ia.asd995.cn

[Q12] 插入后取自增 ID
来源：http://cb.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kb.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gk.521024.cn

[Q13] 忽略重复插入
来源：http://bs.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ya.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://gu.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rx.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ik.bookmarksfly.cn

[Q15] 查询全部
来源：http://iz.chemitech.net.cn

SELECT * FROM users;
来源：http://tk.panjiajie.cn

[Q16] 查询指定列
来源：http://eg.lnxyls.cn

SELECT id, name FROM users;
来源：http://oa.hahajie.cn

[Q17] 条件查询
来源：http://uu.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nr.bjjhwx.cn

[Q18] 模糊匹配
来源：http://oo.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wz.muxihuayi.cn

[Q19] 范围查询
来源：http://ui.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vg.jctech888.com.cn

[Q20] IN 列表
来源：http://zg.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bk.shxzukj.cn

[Q21] 空值判断
来源：http://lb.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://va.asd995.cn

[Q22] 排序
来源：http://pq.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kv.shxzskj.cn

[Q23] 分页
来源：http://lh.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mk.hahajie.cn

[Q24] 去重
来源：http://bz.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://tc.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://dp.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qs.shtwfgs.cn

[Q26] 计数
来源：http://te.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://ya.hahajie.cn

[Q27] 条件计数
来源：http://qg.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pg.newstarts.cn

[Q28] 求和与平均
来源：http://bh.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oi.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://hg.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jctech888.com.cn

[Q30] 分组统计
来源：http://ad.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pr.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://ut.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xp.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://el.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uu.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rs.huixinmuqiang.cn

[Q33] 多列分组
来源：http://sz.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eq.asd995.cn

[Q34] 每组取第一条
来源：http://an.huanxung.cn

SELECT * FROM (
来源：http://qt.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ey.colortex.cn

) t WHERE rn = 1;
来源：http://af.asd995.cn

[Q35] 内连接
来源：http://kz.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nt.bjjhwx.cn

[Q36] 左连接
来源：http://zi.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yx.yuntaijiaju.cn

[Q37] 右连接
来源：http://ct.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gv.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ap.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gm.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://xp.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://js.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wf.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tj.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jt.hnjuh.cn

[Q41] 多表连接
来源：http://gv.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://af.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://yn.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://jk.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://ct.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://pz.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tn.wgjwhj.cn

[Q43] 标量子查询
来源：http://gz.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gu.hnjuh.cn

[Q44] IN 子查询
来源：http://ov.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eu.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://gb.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ql.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sz.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ji.asd995.cn

[Q47] 与平均值比较
来源：http://gb.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cj.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://de.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xi.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://kj.shxzukj.cn

[Q49] 更新单行
来源：http://rg.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bo.panjiajie.cn

[Q50] 批量更新
来源：http://qh.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://he.9csxet.cn

[Q51] 用子查询更新
来源：http://eg.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://me.yuexingan06.cn

[Q52] 删除指定行
来源：http://ka.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://ma.szxytkj.cn

[Q53] 按条件删除
来源：http://vr.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lc.colortex.cn

[Q54] 清空表
来源：http://oa.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://qk.hahajie.cn

[Q55] 排名（并列占位）
来源：http://iv.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vb.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://vb.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ry.hahajie.cn

[Q57] 行号
来源：http://yy.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://co.haigaiapp.cn

[Q58] 累计求和
来源：http://fp.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oy.shxzukj.cn

[Q59] 分组内累计
来源：http://lj.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nh.521024.cn

[Q60] 取上一行 / 下一行
来源：http://lx.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nm.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vm.szxytkj.cn

[Q61] 移动平均
来源：http://gg.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sf.panjiajie.cn

[Q62] 分组占比
来源：http://rf.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ln.asd995.cn

[Q63] 开启事务
来源：http://ny.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mi.asd995.cn

[Q64] 提交事务
来源：http://ug.szsharing.cn

COMMIT;
来源：http://ff.nicolike.cn

[Q65] 回滚事务
来源：http://en.521024.cn

ROLLBACK;
来源：http://to.colortex.cn

[Q66] 行锁查询
来源：http://bt.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wq.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://xz.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xc.shtwfgs.cn

[Q68] 保存点
来源：http://cp.haigaiapp.cn

SAVEPOINT sp1;
来源：http://vr.huanxung.cn

ROLLBACK TO sp1;
来源：http://ce.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://hx.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vk.asd995.cn

[Q70] 更新统计信息
来源：http://ke.szsharing.cn

ANALYZE TABLE users;
来源：http://fv.haigaiapp.cn

[Q71] 查看建表语句
来源：http://la.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cf.panjiajie.cn

[Q72] 查看索引
来源：http://kd.hnjuh.cn

SHOW INDEX FROM users;
来源：http://ai.521024.cn

[Q73] 查看表状态
来源：http://te.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lx.haigaiapp.cn

[Q74] 强制使用索引
来源：http://wv.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gy.bjjhwx.cn

[Q75] 日期格式化
来源：http://wz.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cj.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jp.asd995.cn

[Q76] 按天统计
来源：http://lq.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qa.szxytkj.cn

[Q77] 时间加减
来源：http://rk.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qq.muxihuayi.cn

[Q78] 当前时间
来源：http://oj.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://py.521024.cn

[Q79] 字符串拼接
来源：http://ed.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hn.szxytkj.cn

[Q80] 字符串截取
来源：http://kw.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gv.wgjwhj.cn

[Q81] 字符串替换
来源：http://jw.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fs.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://uv.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jo.hahajie.cn

[Q83] 大小写转换
来源：http://gq.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xm.yuntaijiaju.cn


<!-- 参考信息 -->