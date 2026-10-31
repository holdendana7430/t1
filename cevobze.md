代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://zh.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://dm.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://te.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://eh.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xv.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://gu.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tc.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rp.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bu.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hl.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://ia.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://pz.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://gc.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zp.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://di.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://eq.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qd.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ej.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://vd.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kn.bjjhwx.cn

[O06] 使用进程池
来源：http://he.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mq.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cj.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://vb.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://wq.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cz.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://us.muxihuayi.cn

Ruby: // fork 块
来源：http://sm.huixiangedu.cn

C#:   Parallel.For
来源：http://lb.gzmigu.cn

================================================================================
来源：http://dj.huixinmuqiang.cn

P. 常用工具函数
来源：http://df.hnjuh.cn

================================================================================
来源：http://dc.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://uk.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://bt.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fk.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://gz.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://dm.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://om.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://em.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://qc.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://cl.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://wf.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uk.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nu.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fc.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gs.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jl.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://re.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ra.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xa.gzmigu.cn

[P03] 生成短随机字符串
来源：http://bu.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cc.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ig.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mt.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pg.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pw.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kh.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yt.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yr.shxzukj.cn

[P04] 求长度
来源：http://ug.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jq.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zw.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tu.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gm.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://yb.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://ab.asd995.cn

Ruby: x.length;  x.size
来源：http://ie.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sp.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://rk.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ye.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ym.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wn.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wu.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vk.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://au.chemitech.net.cn

Ruby: a == b
来源：http://zr.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cc.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fr.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cv.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://cx.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://en.asd995.cn

TS:   if (x == null) {}
来源：http://wp.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qq.szsharing.cn

Go:   if x == nil {}
来源：http://qt.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gc.haigaiapp.cn

C#:   if (x is null) {}
来源：http://oz.9csxet.cn

[P07] 防抖与节流
来源：http://mn.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ue.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ge.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gy.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lh.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://it.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hf.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ds.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lt.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://vf.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gt.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dz.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ah.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uy.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gs.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ew.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ty.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wo.jianghongdianzi.cn

================================================================================
来源：http://fy.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qe.nszjky.cn

================================================================================
来源：http://dr.huixinmuqiang.cn

[Q01] 创建表
来源：http://cg.shtwfgs.cn

CREATE TABLE users (
来源：http://cw.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jw.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://qj.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://gy.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bt.szsharing.cn

);
来源：http://ij.nszjky.cn

[Q02] 创建带外键的表
来源：http://cx.szsharing.cn

CREATE TABLE orders (
来源：http://yx.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qq.huixiangedu.cn

user_id INT NOT NULL,
来源：http://du.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://yb.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jk.newstarts.cn

);
来源：http://rv.panjiajie.cn

[Q03] 增加列
来源：http://zv.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gb.szsharing.cn

[Q04] 修改列类型
来源：http://sl.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oj.muxihuayi.cn

[Q05] 重命名列
来源：http://qt.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mr.jctech888.com.cn

[Q06] 删除列
来源：http://tf.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ql.huixinmuqiang.cn

[Q07] 删除表
来源：http://cq.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://bk.nicolike.cn

[Q08] 创建普通索引
来源：http://gf.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vp.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://sl.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://am.panjiajie.cn

[Q10] 插入单行
来源：http://hp.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wi.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://wk.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eb.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://bm.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ed.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uj.shxzskj.cn

[Q13] 忽略重复插入
来源：http://os.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ad.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://vt.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kj.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lj.wgjwhj.cn

[Q15] 查询全部
来源：http://sp.newstarts.cn

SELECT * FROM users;
来源：http://wm.521024.cn

[Q16] 查询指定列
来源：http://sz.hnjuh.cn

SELECT id, name FROM users;
来源：http://za.huixiangedu.cn

[Q17] 条件查询
来源：http://wa.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hn.szsharing.cn

[Q18] 模糊匹配
来源：http://tb.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lh.hnjuh.cn

[Q19] 范围查询
来源：http://op.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://em.asd995.cn

[Q20] IN 列表
来源：http://sc.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nt.szsharing.cn

[Q21] 空值判断
来源：http://pp.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sf.haigaiapp.cn

[Q22] 排序
来源：http://cd.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fh.szxytkj.cn

[Q23] 分页
来源：http://hf.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rl.newstarts.cn

[Q24] 去重
来源：http://fz.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://st.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://gf.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sc.bookmarksfly.cn

[Q26] 计数
来源：http://ga.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://me.yuntaijiaju.cn

[Q27] 条件计数
来源：http://zx.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yo.bjjhwx.cn

[Q28] 求和与平均
来源：http://mt.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kw.huanxung.cn

[Q29] 最大最小值
来源：http://py.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://as.wgjwhj.cn

[Q30] 分组统计
来源：http://js.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mw.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://ln.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vw.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://gl.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lv.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kc.lnxyls.cn

[Q33] 多列分组
来源：http://lw.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vd.yuexingan06.cn

[Q34] 每组取第一条
来源：http://db.nszjky.cn

SELECT * FROM (
来源：http://nm.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ig.muxihuayi.cn

) t WHERE rn = 1;
来源：http://ll.muxihuayi.cn

[Q35] 内连接
来源：http://yw.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wr.nszjky.cn

[Q36] 左连接
来源：http://va.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ws.newstarts.cn

[Q37] 右连接
来源：http://og.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ej.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hy.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iy.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://dj.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wq.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lu.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wg.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://le.huixiangedu.cn

[Q41] 多表连接
来源：http://rt.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vy.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://wo.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://sk.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://rc.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://hi.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pj.shtwfgs.cn

[Q43] 标量子查询
来源：http://co.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gd.szsharing.cn

[Q44] IN 子查询
来源：http://it.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bg.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://no.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xq.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vv.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bl.nicolike.cn

[Q47] 与平均值比较
来源：http://md.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pv.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://tm.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aa.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://sh.chemitech.net.cn

[Q49] 更新单行
来源：http://fw.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kr.bookmarksfly.cn

[Q50] 批量更新
来源：http://yp.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dw.yuexingan06.cn

[Q51] 用子查询更新
来源：http://ak.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gm.nszjky.cn

[Q52] 删除指定行
来源：http://hk.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://ny.shxzukj.cn

[Q53] 按条件删除
来源：http://kc.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pl.asd995.cn

[Q54] 清空表
来源：http://ym.szsharing.cn

TRUNCATE TABLE logs;
来源：http://qe.521024.cn

[Q55] 排名（并列占位）
来源：http://yy.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jp.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://fr.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rh.huanxung.cn

[Q57] 行号
来源：http://mb.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oo.szsharing.cn

[Q58] 累计求和
来源：http://mr.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ob.newstarts.cn

[Q59] 分组内累计
来源：http://dn.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bq.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ik.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ur.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://up.shxzukj.cn

[Q61] 移动平均
来源：http://mo.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nq.newstarts.cn

[Q62] 分组占比
来源：http://hc.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mu.panjiajie.cn

[Q63] 开启事务
来源：http://mv.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yg.shtwfgs.cn

[Q64] 提交事务
来源：http://ho.jctech888.com.cn

COMMIT;
来源：http://qr.bookmarksfly.cn

[Q65] 回滚事务
来源：http://xu.panjiajie.cn

ROLLBACK;
来源：http://se.shtwfgs.cn

[Q66] 行锁查询
来源：http://jt.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ib.hnjuh.cn

[Q67] 设置隔离级别
来源：http://sr.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rt.szxytkj.cn

[Q68] 保存点
来源：http://km.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://ip.nszjky.cn

ROLLBACK TO sp1;
来源：http://ei.huixiangedu.cn

[Q69] 查看执行计划
来源：http://ih.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vf.hahajie.cn

[Q70] 更新统计信息
来源：http://fa.shxzskj.cn

ANALYZE TABLE users;
来源：http://gw.wgjwhj.cn

[Q71] 查看建表语句
来源：http://oh.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jb.jianghongdianzi.cn

[Q72] 查看索引
来源：http://bg.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://ek.haigaiapp.cn

[Q73] 查看表状态
来源：http://ur.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kt.gzmigu.cn

[Q74] 强制使用索引
来源：http://up.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gd.hnjuh.cn

[Q75] 日期格式化
来源：http://hm.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://il.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qy.gzmigu.cn

[Q76] 按天统计
来源：http://bi.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qp.shxzukj.cn

[Q77] 时间加减
来源：http://mf.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://od.hnjuh.cn

[Q78] 当前时间
来源：http://gt.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hi.shxzskj.cn

[Q79] 字符串拼接
来源：http://nj.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qk.colortex.cn

[Q80] 字符串截取
来源：http://ww.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tc.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://hn.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uz.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://nv.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ww.haigaiapp.cn

[Q83] 大小写转换
来源：http://cd.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vm.szsharing.cn

[Q84] 去除首尾空格
来源：http://uu.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://pu.shxzskj.cn

[Q85] 数值取整
来源：http://vu.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ry.haigaiapp.cn


<!-- 参考信息 -->