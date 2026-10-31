代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://ho.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nb.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://cj.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://nm.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yw.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://df.colortex.cn

Ruby: threads.map(&:join)
来源：http://ua.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ba.yuexingan06.cn

[O06] 使用进程池
来源：http://ta.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ex.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wf.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://ft.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://cj.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ua.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xf.shtwfgs.cn

Ruby: // fork 块
来源：http://ov.haigaiapp.cn

C#:   Parallel.For
来源：http://tr.hahajie.cn

================================================================================
来源：http://zu.colortex.cn

P. 常用工具函数
来源：http://nu.yuntaijiaju.cn

================================================================================
来源：http://bf.gzmigu.cn

[P01] 生成 UUID
来源：http://gg.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://fn.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xp.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://jr.nszjky.cn

TS:   crypto.randomUUID()
来源：http://ku.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://fx.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://ef.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://gp.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://cw.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://ar.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iq.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oq.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ys.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dw.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://be.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zs.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rw.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gf.colortex.cn

[P03] 生成短随机字符串
来源：http://es.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ps.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rs.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gi.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qi.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jb.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sj.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dt.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vb.bjjhwx.cn

[P04] 求长度
来源：http://bq.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yq.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kz.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lw.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dx.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://hl.9csxet.cn

Go:   len(arr);  len(m)
来源：http://gw.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://sp.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ke.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://vg.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jm.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ck.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zj.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ra.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sp.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hc.gzmigu.cn

Ruby: a == b
来源：http://en.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iz.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ma.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nn.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://kj.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ur.haigaiapp.cn

TS:   if (x == null) {}
来源：http://qi.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gi.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://ql.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ss.muxihuayi.cn

C#:   if (x is null) {}
来源：http://th.shxzskj.cn

[P07] 防抖与节流
来源：http://ng.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hc.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://je.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hc.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pu.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qv.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aq.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gw.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pm.9csxet.cn

[P08] 处理浮点精度问题
来源：http://rq.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oh.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ww.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ec.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ru.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vb.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hb.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ox.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hc.szsharing.cn

================================================================================
来源：http://ob.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://au.huanxung.cn

================================================================================
来源：http://kw.yuexingan06.cn

[Q01] 创建表
来源：http://ag.muxihuayi.cn

CREATE TABLE users (
来源：http://ob.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gz.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://tx.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://kc.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pl.nszjky.cn

);
来源：http://oo.hahajie.cn

[Q02] 创建带外键的表
来源：http://yr.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://oy.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sc.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://lk.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://uz.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lt.hahajie.cn

);
来源：http://vu.shtwfgs.cn

[Q03] 增加列
来源：http://wo.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://du.bookmarksfly.cn

[Q04] 修改列类型
来源：http://ui.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ic.hnjuh.cn

[Q05] 重命名列
来源：http://fl.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kx.yuntaijiaju.cn

[Q06] 删除列
来源：http://cu.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nf.szxytkj.cn

[Q07] 删除表
来源：http://pl.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://bb.9csxet.cn

[Q08] 创建普通索引
来源：http://lo.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ge.nicolike.cn

[Q09] 创建唯一索引
来源：http://mn.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lj.muxihuayi.cn

[Q10] 插入单行
来源：http://ii.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vi.chemitech.net.cn

[Q11] 一次插入多行
来源：http://th.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vx.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://za.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kc.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hm.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://rd.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dd.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://br.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wf.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uo.panjiajie.cn

[Q15] 查询全部
来源：http://te.colortex.cn

SELECT * FROM users;
来源：http://cf.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://zo.521024.cn

SELECT id, name FROM users;
来源：http://ao.9csxet.cn

[Q17] 条件查询
来源：http://av.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ic.shxzukj.cn

[Q18] 模糊匹配
来源：http://yk.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ut.yuexingan06.cn

[Q19] 范围查询
来源：http://zf.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rc.jctech888.com.cn

[Q20] IN 列表
来源：http://ko.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mq.lnxyls.cn

[Q21] 空值判断
来源：http://cz.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sf.muxihuayi.cn

[Q22] 排序
来源：http://fr.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ft.jctech888.com.cn

[Q23] 分页
来源：http://th.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://br.muxihuayi.cn

[Q24] 去重
来源：http://nu.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://de.nszjky.cn

[Q25] 只取前 N 条
来源：http://oo.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gb.521024.cn

[Q26] 计数
来源：http://tp.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://ec.muxihuayi.cn

[Q27] 条件计数
来源：http://qn.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mm.hnjuh.cn

[Q28] 求和与平均
来源：http://rn.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rh.shxzukj.cn

[Q29] 最大最小值
来源：http://tz.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wq.lnxyls.cn

[Q30] 分组统计
来源：http://mq.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zd.jctech888.com.cn

[Q31] 分组后过滤
来源：http://xd.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dg.521024.cn

[Q32] 分组拼接字符串
来源：http://qi.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lt.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vj.wgjwhj.cn

[Q33] 多列分组
来源：http://wa.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kq.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ps.asd995.cn

SELECT * FROM (
来源：http://jl.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ao.hahajie.cn

) t WHERE rn = 1;
来源：http://ud.shxzukj.cn

[Q35] 内连接
来源：http://ww.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nq.bookmarksfly.cn

[Q36] 左连接
来源：http://fe.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gq.panjiajie.cn

[Q37] 右连接
来源：http://np.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nx.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pg.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://va.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ae.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aw.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://du.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lx.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oo.nicolike.cn

[Q41] 多表连接
来源：http://yg.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://le.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://rc.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ya.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://vc.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://qd.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ta.colortex.cn

[Q43] 标量子查询
来源：http://mx.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bj.yuexingan06.cn

[Q44] IN 子查询
来源：http://dl.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uf.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://fc.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fs.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fc.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rc.shtwfgs.cn

[Q47] 与平均值比较
来源：http://fr.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ds.521024.cn

[Q48] CTE 公用表表达式
来源：http://ff.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dm.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ik.haigaiapp.cn

[Q49] 更新单行
来源：http://by.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wk.yuntaijiaju.cn

[Q50] 批量更新
来源：http://ef.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://in.haigaiapp.cn

[Q51] 用子查询更新
来源：http://kb.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jn.shxzskj.cn

[Q52] 删除指定行
来源：http://og.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://fm.nszjky.cn

[Q53] 按条件删除
来源：http://bv.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ex.nszjky.cn

[Q54] 清空表
来源：http://zq.nicolike.cn

TRUNCATE TABLE logs;
来源：http://wo.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://yy.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lr.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://py.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pc.huixiangedu.cn

[Q57] 行号
来源：http://nj.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fv.asd995.cn

[Q58] 累计求和
来源：http://lh.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dn.szsharing.cn

[Q59] 分组内累计
来源：http://yy.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://np.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://ck.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rt.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bf.huixiangedu.cn

[Q61] 移动平均
来源：http://cm.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fv.hnjuh.cn

[Q62] 分组占比
来源：http://mm.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bz.jianghongdianzi.cn

[Q63] 开启事务
来源：http://ab.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yd.nszjky.cn

[Q64] 提交事务
来源：http://gz.shxzskj.cn

COMMIT;
来源：http://uj.szsharing.cn

[Q65] 回滚事务
来源：http://eo.nicolike.cn

ROLLBACK;
来源：http://su.521024.cn

[Q66] 行锁查询
来源：http://xw.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bd.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://ip.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cr.jianghongdianzi.cn

[Q68] 保存点
来源：http://yl.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://pj.521024.cn

ROLLBACK TO sp1;
来源：http://sb.hahajie.cn

[Q69] 查看执行计划
来源：http://ao.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xg.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://rc.colortex.cn

ANALYZE TABLE users;
来源：http://kr.newstarts.cn

[Q71] 查看建表语句
来源：http://rn.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ft.bjjhwx.cn

[Q72] 查看索引
来源：http://qy.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://le.chemitech.net.cn

[Q73] 查看表状态
来源：http://ug.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ih.szsharing.cn

[Q74] 强制使用索引
来源：http://fr.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ye.wgjwhj.cn

[Q75] 日期格式化
来源：http://zw.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zj.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ce.9csxet.cn

[Q76] 按天统计
来源：http://vu.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dc.huixinmuqiang.cn

[Q77] 时间加减
来源：http://vw.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sw.9csxet.cn

[Q78] 当前时间
来源：http://jx.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xe.wgjwhj.cn

[Q79] 字符串拼接
来源：http://wv.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sp.hahajie.cn

[Q80] 字符串截取
来源：http://vh.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mw.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://yf.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gi.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://vi.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vq.huanxung.cn

[Q83] 大小写转换
来源：http://hl.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ak.szxytkj.cn

[Q84] 去除首尾空格
来源：http://fk.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://av.newstarts.cn

[Q85] 数值取整
来源：http://ul.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pn.colortex.cn

[Q86] 读取 JSON 字段
来源：http://to.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.asd995.cn

[Q87] JSON 字段做条件
来源：http://jz.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sv.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://qx.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://al.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ec.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://lv.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kl.huanxung.cn

[Q90] 生成序号列
来源：http://pl.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://po.asd995.cn

================================================================================
来源：http://dt.newstarts.cn


<!-- 参考信息 -->