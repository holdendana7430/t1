代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://ze.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jd.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://vb.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://hj.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gl.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tm.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://jo.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oz.nszjky.cn

[O06] 使用进程池
来源：http://fs.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dj.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tn.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://nb.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://am.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bl.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vu.lnxyls.cn

Ruby: // fork 块
来源：http://he.jctech888.com.cn

C#:   Parallel.For
来源：http://cm.jctech888.com.cn

================================================================================
来源：http://ln.huanxung.cn

P. 常用工具函数
来源：http://mk.shxzskj.cn

================================================================================
来源：http://pl.newstarts.cn

[P01] 生成 UUID
来源：http://uz.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://md.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oy.szsharing.cn

JS:   crypto.randomUUID()
来源：http://zh.nszjky.cn

TS:   crypto.randomUUID()
来源：http://re.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://cv.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://xi.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://kt.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://fr.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://iw.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zv.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tp.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oo.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bl.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ej.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ud.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qw.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tr.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://hg.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vx.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fd.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cx.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xk.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yy.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kj.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://su.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gq.hnjuh.cn

[P04] 求长度
来源：http://jv.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iq.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vk.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ix.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ze.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://dr.newstarts.cn

Go:   len(arr);  len(m)
来源：http://mv.newstarts.cn

Ruby: x.length;  x.size
来源：http://ve.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://py.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://gj.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qj.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gg.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pn.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xt.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://js.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://do.shxzukj.cn

Ruby: a == b
来源：http://sd.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eb.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fj.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dh.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://ba.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://se.muxihuayi.cn

TS:   if (x == null) {}
来源：http://nv.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nm.muxihuayi.cn

Go:   if x == nil {}
来源：http://ul.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ky.9csxet.cn

C#:   if (x is null) {}
来源：http://bx.huixiangedu.cn

[P07] 防抖与节流
来源：http://up.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vz.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://he.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kr.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nv.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xz.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vo.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fi.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://uh.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vs.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cp.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cw.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ag.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kz.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hx.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wn.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tk.shtwfgs.cn

================================================================================
来源：http://tm.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lj.huixiangedu.cn

================================================================================
来源：http://nh.wgjwhj.cn

[Q01] 创建表
来源：http://uf.nszjky.cn

CREATE TABLE users (
来源：http://qk.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gh.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://js.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://pz.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sq.huixinmuqiang.cn

);
来源：http://tv.lnxyls.cn

[Q02] 创建带外键的表
来源：http://wg.shtwfgs.cn

CREATE TABLE orders (
来源：http://lu.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gr.hahajie.cn

user_id INT NOT NULL,
来源：http://kb.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://bg.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nj.colortex.cn

);
来源：http://kh.haigaiapp.cn

[Q03] 增加列
来源：http://wm.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ig.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://nj.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ox.yuntaijiaju.cn

[Q05] 重命名列
来源：http://gm.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ct.szsharing.cn

[Q06] 删除列
来源：http://jo.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yl.shxzskj.cn

[Q07] 删除表
来源：http://ry.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://rf.jctech888.com.cn

[Q08] 创建普通索引
来源：http://rl.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nq.nszjky.cn

[Q09] 创建唯一索引
来源：http://vw.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kn.szxytkj.cn

[Q10] 插入单行
来源：http://fk.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sd.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://wy.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gx.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://ez.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jc.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sq.lnxyls.cn

[Q13] 忽略重复插入
来源：http://bi.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dd.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://bt.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ss.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xz.newstarts.cn

[Q15] 查询全部
来源：http://mf.yuntaijiaju.cn

SELECT * FROM users;
来源：http://qg.hahajie.cn

[Q16] 查询指定列
来源：http://ou.wgjwhj.cn

SELECT id, name FROM users;
来源：http://si.huixinmuqiang.cn

[Q17] 条件查询
来源：http://hl.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mv.hnjuh.cn

[Q18] 模糊匹配
来源：http://lk.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fp.jianghongdianzi.cn

[Q19] 范围查询
来源：http://wg.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hc.jianghongdianzi.cn

[Q20] IN 列表
来源：http://mh.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://th.jianghongdianzi.cn

[Q21] 空值判断
来源：http://jy.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zs.szxytkj.cn

[Q22] 排序
来源：http://me.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sr.jctech888.com.cn

[Q23] 分页
来源：http://jv.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pd.panjiajie.cn

[Q24] 去重
来源：http://al.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://mw.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://xg.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sj.haigaiapp.cn

[Q26] 计数
来源：http://al.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://qm.nicolike.cn

[Q27] 条件计数
来源：http://pf.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ue.bookmarksfly.cn

[Q28] 求和与平均
来源：http://pf.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ml.panjiajie.cn

[Q29] 最大最小值
来源：http://gk.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ik.shxzskj.cn

[Q30] 分组统计
来源：http://ms.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bv.colortex.cn

[Q31] 分组后过滤
来源：http://bw.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://me.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://yv.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jh.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://na.nicolike.cn

[Q33] 多列分组
来源：http://ea.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vy.wgjwhj.cn

[Q34] 每组取第一条
来源：http://iy.colortex.cn

SELECT * FROM (
来源：http://ov.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ic.panjiajie.cn

) t WHERE rn = 1;
来源：http://es.asd995.cn

[Q35] 内连接
来源：http://ji.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hv.huixinmuqiang.cn

[Q36] 左连接
来源：http://jv.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ad.wgjwhj.cn

[Q37] 右连接
来源：http://id.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://er.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kh.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tg.asd995.cn

[Q39] 自连接（查上下级）
来源：http://dx.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sv.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vh.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ui.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dq.lnxyls.cn

[Q41] 多表连接
来源：http://tx.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tz.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://sa.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://mv.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://uc.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://fk.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ln.nszjky.cn

[Q43] 标量子查询
来源：http://ju.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://as.hahajie.cn

[Q44] IN 子查询
来源：http://zk.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gq.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://ao.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pk.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://th.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mj.huanxung.cn

[Q47] 与平均值比较
来源：http://ez.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zf.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://rh.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cw.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://gw.muxihuayi.cn

[Q49] 更新单行
来源：http://yd.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tu.szsharing.cn

[Q50] 批量更新
来源：http://un.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://is.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://eh.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ez.szxytkj.cn

[Q52] 删除指定行
来源：http://mr.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://dq.newstarts.cn

[Q53] 按条件删除
来源：http://cy.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jr.nszjky.cn

[Q54] 清空表
来源：http://ya.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://xu.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://sw.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ts.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://yv.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://of.bookmarksfly.cn

[Q57] 行号
来源：http://gk.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zt.hahajie.cn

[Q58] 累计求和
来源：http://hr.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sw.gzmigu.cn

[Q59] 分组内累计
来源：http://kl.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dz.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://tn.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bo.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lq.bjjhwx.cn

[Q61] 移动平均
来源：http://nf.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hs.yuexingan06.cn

[Q62] 分组占比
来源：http://bl.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sc.panjiajie.cn

[Q63] 开启事务
来源：http://bq.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uw.521024.cn

[Q64] 提交事务
来源：http://wq.bjjhwx.cn

COMMIT;
来源：http://kw.muxihuayi.cn

[Q65] 回滚事务
来源：http://zc.huanxung.cn

ROLLBACK;
来源：http://oi.yuexingan06.cn

[Q66] 行锁查询
来源：http://ws.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qd.colortex.cn

[Q67] 设置隔离级别
来源：http://bn.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ka.jctech888.com.cn

[Q68] 保存点
来源：http://qp.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://eh.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://me.chemitech.net.cn

[Q69] 查看执行计划
来源：http://xj.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uk.521024.cn

[Q70] 更新统计信息
来源：http://zo.szsharing.cn

ANALYZE TABLE users;
来源：http://pe.haigaiapp.cn

[Q71] 查看建表语句
来源：http://wi.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://py.yuexingan06.cn

[Q72] 查看索引
来源：http://tt.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://vo.shxzukj.cn

[Q73] 查看表状态
来源：http://qf.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bf.hahajie.cn

[Q74] 强制使用索引
来源：http://gx.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zh.bookmarksfly.cn

[Q75] 日期格式化
来源：http://dx.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fp.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kv.nicolike.cn

[Q76] 按天统计
来源：http://gy.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wo.jianghongdianzi.cn

[Q77] 时间加减
来源：http://cq.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zi.huanxung.cn

[Q78] 当前时间
来源：http://jp.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://he.gzmigu.cn

[Q79] 字符串拼接
来源：http://if.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hn.bjjhwx.cn

[Q80] 字符串截取
来源：http://az.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zm.nszjky.cn

[Q81] 字符串替换
来源：http://hw.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pf.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://ro.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tq.9csxet.cn

[Q83] 大小写转换
来源：http://vq.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wo.shxzskj.cn

[Q84] 去除首尾空格
来源：http://ur.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://lg.huixinmuqiang.cn

[Q85] 数值取整
来源：http://pj.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dr.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://ff.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wq.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://qx.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mh.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://sv.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lj.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qb.521024.cn

[Q89] 判断表是否存在
来源：http://ie.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bw.muxihuayi.cn

[Q90] 生成序号列
来源：http://ku.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yz.lnxyls.cn

================================================================================
来源：http://fg.huanxung.cn


<!-- 参考信息 -->