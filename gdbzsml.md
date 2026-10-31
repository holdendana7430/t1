代发 wailian999

[O06] 使用进程池
来源：http://sk.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nf.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ew.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://fm.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://fo.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jx.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gw.huixinmuqiang.cn

Ruby: // fork 块
来源：http://wa.asd995.cn

C#:   Parallel.For
来源：http://la.szxytkj.cn

================================================================================
来源：http://zq.muxihuayi.cn

P. 常用工具函数
来源：http://ls.hahajie.cn

================================================================================
来源：http://lo.szxytkj.cn

[P01] 生成 UUID
来源：http://rd.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://tp.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bv.newstarts.cn

JS:   crypto.randomUUID()
来源：http://dv.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://mc.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://ki.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://pj.colortex.cn

Ruby: SecureRandom.uuid
来源：http://jk.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://wg.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://gd.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pc.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tj.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mt.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uf.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tc.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mr.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://at.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lp.panjiajie.cn

[P03] 生成短随机字符串
来源：http://wf.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xl.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fz.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ja.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ha.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mn.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://il.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xx.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sn.asd995.cn

[P04] 求长度
来源：http://ia.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fv.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ug.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cg.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pm.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://cr.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://ak.colortex.cn

Ruby: x.length;  x.size
来源：http://vn.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yv.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://zw.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ss.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dc.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vj.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://co.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jc.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qx.chemitech.net.cn

Ruby: a == b
来源：http://yd.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iw.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fj.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kl.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://gg.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://af.panjiajie.cn

TS:   if (x == null) {}
来源：http://yl.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uo.yuexingan06.cn

Go:   if x == nil {}
来源：http://rb.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yk.521024.cn

C#:   if (x is null) {}
来源：http://vw.lnxyls.cn

[P07] 防抖与节流
来源：http://ad.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://we.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://cz.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://og.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yo.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ec.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iy.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fu.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gj.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://pp.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jn.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ch.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eg.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uv.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rg.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mx.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zy.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dg.hahajie.cn

================================================================================
来源：http://ow.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wo.huixinmuqiang.cn

================================================================================
来源：http://zp.lnxyls.cn

[Q01] 创建表
来源：http://ok.nszjky.cn

CREATE TABLE users (
来源：http://yk.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nv.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ic.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://jf.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nh.shxzukj.cn

);
来源：http://zq.panjiajie.cn

[Q02] 创建带外键的表
来源：http://cr.shxzskj.cn

CREATE TABLE orders (
来源：http://dk.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sz.szxytkj.cn

user_id INT NOT NULL,
来源：http://jj.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://qk.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vz.gzmigu.cn

);
来源：http://nn.jianghongdianzi.cn

[Q03] 增加列
来源：http://kb.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cl.hnjuh.cn

[Q04] 修改列类型
来源：http://ga.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gw.szsharing.cn

[Q05] 重命名列
来源：http://qw.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://at.nicolike.cn

[Q06] 删除列
来源：http://rp.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kk.bookmarksfly.cn

[Q07] 删除表
来源：http://xz.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://gq.panjiajie.cn

[Q08] 创建普通索引
来源：http://ks.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://td.nszjky.cn

[Q09] 创建唯一索引
来源：http://pp.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cf.newstarts.cn

[Q10] 插入单行
来源：http://mt.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uj.asd995.cn

[Q11] 一次插入多行
来源：http://qk.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lo.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://sp.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ac.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ay.hahajie.cn

[Q13] 忽略重复插入
来源：http://rv.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://as.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://yg.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fj.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mz.huanxung.cn

[Q15] 查询全部
来源：http://sw.shxzukj.cn

SELECT * FROM users;
来源：http://px.shtwfgs.cn

[Q16] 查询指定列
来源：http://uy.jctech888.com.cn

SELECT id, name FROM users;
来源：http://jp.nszjky.cn

[Q17] 条件查询
来源：http://se.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kr.9csxet.cn

[Q18] 模糊匹配
来源：http://mf.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ai.nszjky.cn

[Q19] 范围查询
来源：http://oo.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nv.haigaiapp.cn

[Q20] IN 列表
来源：http://sm.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dh.521024.cn

[Q21] 空值判断
来源：http://ph.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zy.huixiangedu.cn

[Q22] 排序
来源：http://tz.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hy.jctech888.com.cn

[Q23] 分页
来源：http://yu.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ub.jctech888.com.cn

[Q24] 去重
来源：http://ls.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://yt.huanxung.cn

[Q25] 只取前 N 条
来源：http://ja.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sx.wgjwhj.cn

[Q26] 计数
来源：http://ct.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://ta.huanxung.cn

[Q27] 条件计数
来源：http://qv.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ye.nszjky.cn

[Q28] 求和与平均
来源：http://gt.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lt.yuexingan06.cn

[Q29] 最大最小值
来源：http://lh.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ix.asd995.cn

[Q30] 分组统计
来源：http://oc.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ja.hnjuh.cn

[Q31] 分组后过滤
来源：http://br.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vt.szsharing.cn

[Q32] 分组拼接字符串
来源：http://dy.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vo.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bv.huanxung.cn

[Q33] 多列分组
来源：http://nb.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xx.asd995.cn

[Q34] 每组取第一条
来源：http://cc.panjiajie.cn

SELECT * FROM (
来源：http://fi.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sg.jctech888.com.cn

) t WHERE rn = 1;
来源：http://ai.jianghongdianzi.cn

[Q35] 内连接
来源：http://cz.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yd.521024.cn

[Q36] 左连接
来源：http://kj.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ew.bookmarksfly.cn

[Q37] 右连接
来源：http://so.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jd.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qj.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zy.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://ow.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ig.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hw.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pv.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cc.colortex.cn

[Q41] 多表连接
来源：http://oo.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gj.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://tx.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://bt.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://qi.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://wh.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zu.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://ap.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://be.jctech888.com.cn

[Q44] IN 子查询
来源：http://ca.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hi.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://fe.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jf.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ef.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://do.colortex.cn

[Q47] 与平均值比较
来源：http://xj.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zh.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://sw.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jr.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://sq.szxytkj.cn

[Q49] 更新单行
来源：http://ii.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://si.yuexingan06.cn

[Q50] 批量更新
来源：http://iu.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uh.huixiangedu.cn

[Q51] 用子查询更新
来源：http://uz.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://se.bjjhwx.cn

[Q52] 删除指定行
来源：http://lo.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://ka.newstarts.cn

[Q53] 按条件删除
来源：http://ar.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://io.chemitech.net.cn

[Q54] 清空表
来源：http://gz.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://dz.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://td.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qa.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://uf.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fr.9csxet.cn

[Q57] 行号
来源：http://qf.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://op.muxihuayi.cn

[Q58] 累计求和
来源：http://rk.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uj.szxytkj.cn

[Q59] 分组内累计
来源：http://hh.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://np.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://qh.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sc.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mb.yuntaijiaju.cn

[Q61] 移动平均
来源：http://wq.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zs.shxzukj.cn

[Q62] 分组占比
来源：http://hh.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cs.muxihuayi.cn

[Q63] 开启事务
来源：http://nt.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bl.9csxet.cn

[Q64] 提交事务
来源：http://ye.gzmigu.cn

COMMIT;
来源：http://cq.9csxet.cn

[Q65] 回滚事务
来源：http://lj.bjjhwx.cn

ROLLBACK;
来源：http://hi.9csxet.cn

[Q66] 行锁查询
来源：http://yd.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lj.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://tl.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fo.gzmigu.cn

[Q68] 保存点
来源：http://ln.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ae.hnjuh.cn

ROLLBACK TO sp1;
来源：http://gm.hahajie.cn

[Q69] 查看执行计划
来源：http://hy.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wk.newstarts.cn

[Q70] 更新统计信息
来源：http://im.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://xk.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://tz.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oh.hnjuh.cn

[Q72] 查看索引
来源：http://ao.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://kj.chemitech.net.cn

[Q73] 查看表状态
来源：http://zg.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gu.nicolike.cn

[Q74] 强制使用索引
来源：http://ve.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xd.panjiajie.cn

[Q75] 日期格式化
来源：http://pv.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xy.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sc.shtwfgs.cn

[Q76] 按天统计
来源：http://hx.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pi.asd995.cn

[Q77] 时间加减
来源：http://ff.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wf.hnjuh.cn

[Q78] 当前时间
来源：http://dz.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wu.bjjhwx.cn

[Q79] 字符串拼接
来源：http://gi.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gh.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://xa.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sr.panjiajie.cn

[Q81] 字符串替换
来源：http://fj.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kp.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://xi.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zk.yuexingan06.cn

[Q83] 大小写转换
来源：http://rn.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vz.panjiajie.cn

[Q84] 去除首尾空格
来源：http://ro.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://tg.jianghongdianzi.cn

[Q85] 数值取整
来源：http://ck.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tx.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://cw.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hg.9csxet.cn

[Q87] JSON 字段做条件
来源：http://tv.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sg.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://yj.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zc.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pk.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://vh.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hc.gzmigu.cn

[Q90] 生成序号列
来源：http://dx.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ot.gzmigu.cn

================================================================================
来源：http://er.lnxyls.cn

R. Bash 专题
来源：http://yn.szsharing.cn

================================================================================
来源：http://jx.szxytkj.cn

[R01] shebang 与严格模式
来源：http://xp.newstarts.cn

#!/usr/bin/env bash
来源：http://ok.muxihuayi.cn

set -euo pipefail
来源：http://yp.huanxung.cn

[R02] 变量赋值与使用
来源：http://vi.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://gd.hahajie.cn

[R03] 只读变量
来源：http://dl.wgjwhj.cn


<!-- 参考信息 -->