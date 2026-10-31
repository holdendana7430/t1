代发 wailian999

TS:   // child_process / cluster 模块
来源：http://jc.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lk.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eg.szxytkj.cn

Ruby: // fork 块
来源：http://ni.bookmarksfly.cn

C#:   Parallel.For
来源：http://tj.yuntaijiaju.cn

================================================================================
来源：http://en.lnxyls.cn

P. 常用工具函数
来源：http://wh.jianghongdianzi.cn

================================================================================
来源：http://mr.jctech888.com.cn

[P01] 生成 UUID
来源：http://cw.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://di.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vy.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://uq.newstarts.cn

TS:   crypto.randomUUID()
来源：http://mf.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://cd.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://fn.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://pn.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://mc.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://em.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ub.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rb.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://km.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ud.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zn.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ap.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rg.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iz.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://ae.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fe.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dt.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yt.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ih.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ep.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ir.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wf.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dm.szsharing.cn

[P04] 求长度
来源：http://ya.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://de.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ea.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qt.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cm.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://km.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://bf.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://ua.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uh.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://qf.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://by.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qg.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xd.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ti.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://me.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yb.jctech888.com.cn

Ruby: a == b
来源：http://cf.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ux.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lu.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nt.asd995.cn

PHP:  if (empty($x)) {}
来源：http://id.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bh.haigaiapp.cn

TS:   if (x == null) {}
来源：http://cn.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pl.nicolike.cn

Go:   if x == nil {}
来源：http://ll.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ap.521024.cn

C#:   if (x is null) {}
来源：http://xh.szsharing.cn

[P07] 防抖与节流
来源：http://qb.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sn.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://ko.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ly.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lr.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oi.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pm.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qe.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zq.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://dv.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://or.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vv.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://un.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gj.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kb.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dz.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cd.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hm.yuexingan06.cn

================================================================================
来源：http://op.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bm.wgjwhj.cn

================================================================================
来源：http://oj.jctech888.com.cn

[Q01] 创建表
来源：http://pi.yuexingan06.cn

CREATE TABLE users (
来源：http://yn.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cl.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://la.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://hg.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ao.hahajie.cn

);
来源：http://cv.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://vi.hahajie.cn

CREATE TABLE orders (
来源：http://gs.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fl.shxzskj.cn

user_id INT NOT NULL,
来源：http://bp.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://vf.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ya.hnjuh.cn

);
来源：http://uy.bjjhwx.cn

[Q03] 增加列
来源：http://dy.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sb.muxihuayi.cn

[Q04] 修改列类型
来源：http://zk.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lq.haigaiapp.cn

[Q05] 重命名列
来源：http://iv.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ie.wgjwhj.cn

[Q06] 删除列
来源：http://gw.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zh.muxihuayi.cn

[Q07] 删除表
来源：http://uj.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://kg.bjjhwx.cn

[Q08] 创建普通索引
来源：http://bj.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oj.hnjuh.cn

[Q09] 创建唯一索引
来源：http://pf.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wq.haigaiapp.cn

[Q10] 插入单行
来源：http://sj.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cg.nicolike.cn

[Q11] 一次插入多行
来源：http://ca.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hm.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://cq.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sg.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://at.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://oy.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ph.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://ef.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ka.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yx.yuntaijiaju.cn

[Q15] 查询全部
来源：http://xy.szxytkj.cn

SELECT * FROM users;
来源：http://jf.shxzukj.cn

[Q16] 查询指定列
来源：http://qn.nicolike.cn

SELECT id, name FROM users;
来源：http://pn.huixiangedu.cn

[Q17] 条件查询
来源：http://va.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dj.shtwfgs.cn

[Q18] 模糊匹配
来源：http://gq.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ev.panjiajie.cn

[Q19] 范围查询
来源：http://mu.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oy.bookmarksfly.cn

[Q20] IN 列表
来源：http://qx.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://om.gzmigu.cn

[Q21] 空值判断
来源：http://in.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zr.nszjky.cn

[Q22] 排序
来源：http://fb.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://db.colortex.cn

[Q23] 分页
来源：http://lo.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tc.muxihuayi.cn

[Q24] 去重
来源：http://lp.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://fc.nicolike.cn

[Q25] 只取前 N 条
来源：http://km.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gk.hnjuh.cn

[Q26] 计数
来源：http://zl.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://nt.yuexingan06.cn

[Q27] 条件计数
来源：http://sd.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oe.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://rw.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ho.szsharing.cn

[Q29] 最大最小值
来源：http://zr.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nd.yuntaijiaju.cn

[Q30] 分组统计
来源：http://rg.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://af.panjiajie.cn

[Q31] 分组后过滤
来源：http://po.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tj.9csxet.cn

[Q32] 分组拼接字符串
来源：http://tb.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yz.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kr.haigaiapp.cn

[Q33] 多列分组
来源：http://qp.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ip.nicolike.cn

[Q34] 每组取第一条
来源：http://ox.shxzskj.cn

SELECT * FROM (
来源：http://zp.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ze.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://pz.asd995.cn

[Q35] 内连接
来源：http://ih.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ka.hnjuh.cn

[Q36] 左连接
来源：http://bo.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ka.bjjhwx.cn

[Q37] 右连接
来源：http://ex.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vk.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dh.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pw.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://qf.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qq.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vs.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sh.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://du.nicolike.cn

[Q41] 多表连接
来源：http://gj.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vt.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://fa.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://sf.521024.cn

[Q42] 连接条件附加过滤
来源：http://ko.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://wk.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yx.nicolike.cn

[Q43] 标量子查询
来源：http://bn.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ji.hahajie.cn

[Q44] IN 子查询
来源：http://nw.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yz.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://sv.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fn.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rh.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bp.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://fx.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ha.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://ur.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rg.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://mi.wgjwhj.cn

[Q49] 更新单行
来源：http://jh.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ux.nszjky.cn

[Q50] 批量更新
来源：http://xw.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jv.haigaiapp.cn

[Q51] 用子查询更新
来源：http://st.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gz.shtwfgs.cn

[Q52] 删除指定行
来源：http://nm.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://ic.yuexingan06.cn

[Q53] 按条件删除
来源：http://vv.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zv.hahajie.cn

[Q54] 清空表
来源：http://si.nicolike.cn

TRUNCATE TABLE logs;
来源：http://es.szsharing.cn

[Q55] 排名（并列占位）
来源：http://xx.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bv.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://an.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ip.9csxet.cn

[Q57] 行号
来源：http://rj.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ej.newstarts.cn

[Q58] 累计求和
来源：http://mk.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vp.colortex.cn

[Q59] 分组内累计
来源：http://tu.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nc.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://mi.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sb.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bk.jianghongdianzi.cn

[Q61] 移动平均
来源：http://eh.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pu.nicolike.cn

[Q62] 分组占比
来源：http://bq.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qs.yuntaijiaju.cn

[Q63] 开启事务
来源：http://cu.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lv.chemitech.net.cn

[Q64] 提交事务
来源：http://qr.huixiangedu.cn

COMMIT;
来源：http://bj.hnjuh.cn

[Q65] 回滚事务
来源：http://ar.jctech888.com.cn

ROLLBACK;
来源：http://tb.hnjuh.cn

[Q66] 行锁查询
来源：http://eb.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hp.9csxet.cn

[Q67] 设置隔离级别
来源：http://ne.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hb.huixinmuqiang.cn

[Q68] 保存点
来源：http://ct.lnxyls.cn

SAVEPOINT sp1;
来源：http://sz.gzmigu.cn

ROLLBACK TO sp1;
来源：http://oy.huixiangedu.cn

[Q69] 查看执行计划
来源：http://wo.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mq.wgjwhj.cn

[Q70] 更新统计信息
来源：http://hl.szsharing.cn

ANALYZE TABLE users;
来源：http://ox.shxzskj.cn

[Q71] 查看建表语句
来源：http://ri.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xj.hnjuh.cn

[Q72] 查看索引
来源：http://tn.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://mg.nicolike.cn

[Q73] 查看表状态
来源：http://ct.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wo.muxihuayi.cn

[Q74] 强制使用索引
来源：http://rg.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wn.hahajie.cn

[Q75] 日期格式化
来源：http://ad.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bi.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://di.hnjuh.cn

[Q76] 按天统计
来源：http://jf.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ao.lnxyls.cn

[Q77] 时间加减
来源：http://om.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fy.hahajie.cn

[Q78] 当前时间
来源：http://ez.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cr.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://el.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eg.muxihuayi.cn

[Q80] 字符串截取
来源：http://bn.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ct.nicolike.cn

[Q81] 字符串替换
来源：http://wj.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nv.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://nt.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://md.chemitech.net.cn

[Q83] 大小写转换
来源：http://qj.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kc.hnjuh.cn

[Q84] 去除首尾空格
来源：http://qq.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://nz.haigaiapp.cn

[Q85] 数值取整
来源：http://hj.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://te.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://kv.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ja.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://it.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yq.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://pe.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nt.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://my.newstarts.cn

[Q89] 判断表是否存在
来源：http://dd.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://em.nicolike.cn

[Q90] 生成序号列
来源：http://wt.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qg.colortex.cn

================================================================================
来源：http://br.hahajie.cn

R. Bash 专题
来源：http://kj.panjiajie.cn

================================================================================
来源：http://wa.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://xg.nszjky.cn

#!/usr/bin/env bash
来源：http://mt.newstarts.cn

set -euo pipefail
来源：http://vk.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://dr.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://dt.hahajie.cn

[R03] 只读变量
来源：http://vl.huixiangedu.cn

readonly PI=3.14
来源：http://lq.panjiajie.cn

[R04] 位置参数
来源：http://tq.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bp.lnxyls.cn

[R05] 参数默认值
来源：http://zg.szxytkj.cn


<!-- 参考信息 -->