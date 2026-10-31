代发 wailian999

C#:   Parallel.For
来源：http://te.jianghongdianzi.cn

================================================================================
来源：http://he.yuexingan06.cn

P. 常用工具函数
来源：http://fn.colortex.cn

================================================================================
来源：http://hj.haigaiapp.cn

[P01] 生成 UUID
来源：http://kc.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://tr.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cs.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://xv.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://jd.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://ip.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://gs.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://cw.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://ni.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://ef.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fm.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bd.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ux.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vm.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mo.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pt.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://go.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hd.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://um.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lf.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qg.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rp.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vs.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sg.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ks.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ii.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ed.hnjuh.cn

[P04] 求长度
来源：http://lc.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tg.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bx.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://js.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jb.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://bv.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://jd.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://hq.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nk.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://jf.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xo.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ia.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cr.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fd.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ws.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yh.newstarts.cn

Ruby: a == b
来源：http://xf.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gz.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mg.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://di.colortex.cn

PHP:  if (empty($x)) {}
来源：http://nc.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bu.lnxyls.cn

TS:   if (x == null) {}
来源：http://mr.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lv.shtwfgs.cn

Go:   if x == nil {}
来源：http://pe.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jf.lnxyls.cn

C#:   if (x is null) {}
来源：http://sk.wgjwhj.cn

[P07] 防抖与节流
来源：http://ns.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qc.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://eu.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yj.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ew.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pb.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://up.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fn.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://lf.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://me.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yj.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qz.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ma.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ja.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pq.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qa.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bu.nszjky.cn

================================================================================
来源：http://tz.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pr.gzmigu.cn

================================================================================
来源：http://bl.yuexingan06.cn

[Q01] 创建表
来源：http://kv.521024.cn

CREATE TABLE users (
来源：http://pz.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kv.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://jc.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://yp.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aj.shxzukj.cn

);
来源：http://ow.nszjky.cn

[Q02] 创建带外键的表
来源：http://aa.panjiajie.cn

CREATE TABLE orders (
来源：http://dp.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://am.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://lt.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://bf.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cm.yuexingan06.cn

);
来源：http://cq.gzmigu.cn

[Q03] 增加列
来源：http://am.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wz.hahajie.cn

[Q04] 修改列类型
来源：http://hp.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cm.yuexingan06.cn

[Q05] 重命名列
来源：http://aq.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dj.bookmarksfly.cn

[Q06] 删除列
来源：http://tu.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ar.huixinmuqiang.cn

[Q07] 删除表
来源：http://vn.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://qz.huanxung.cn

[Q08] 创建普通索引
来源：http://mv.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://of.szsharing.cn

[Q09] 创建唯一索引
来源：http://zj.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kd.szxytkj.cn

[Q10] 插入单行
来源：http://ik.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lv.nicolike.cn

[Q11] 一次插入多行
来源：http://jg.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mp.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://ip.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tm.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vr.szxytkj.cn

[Q13] 忽略重复插入
来源：http://im.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sx.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://ti.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ad.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ey.huanxung.cn

[Q15] 查询全部
来源：http://be.hahajie.cn

SELECT * FROM users;
来源：http://gt.gzmigu.cn

[Q16] 查询指定列
来源：http://je.haigaiapp.cn

SELECT id, name FROM users;
来源：http://qw.szsharing.cn

[Q17] 条件查询
来源：http://lt.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kb.lnxyls.cn

[Q18] 模糊匹配
来源：http://xk.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xq.bjjhwx.cn

[Q19] 范围查询
来源：http://ul.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lq.newstarts.cn

[Q20] IN 列表
来源：http://gm.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://or.panjiajie.cn

[Q21] 空值判断
来源：http://mh.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dt.521024.cn

[Q22] 排序
来源：http://mw.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ll.huixinmuqiang.cn

[Q23] 分页
来源：http://mp.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ow.yuexingan06.cn

[Q24] 去重
来源：http://pn.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://fr.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://xn.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ct.chemitech.net.cn

[Q26] 计数
来源：http://ya.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://cx.shxzskj.cn

[Q27] 条件计数
来源：http://rp.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qp.hnjuh.cn

[Q28] 求和与平均
来源：http://mz.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qo.shxzskj.cn

[Q29] 最大最小值
来源：http://bu.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kj.yuexingan06.cn

[Q30] 分组统计
来源：http://yc.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ga.haigaiapp.cn

[Q31] 分组后过滤
来源：http://qz.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ua.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://so.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lg.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ow.yuexingan06.cn

[Q33] 多列分组
来源：http://hi.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yt.newstarts.cn

[Q34] 每组取第一条
来源：http://ul.panjiajie.cn

SELECT * FROM (
来源：http://hf.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://an.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://kf.yuexingan06.cn

[Q35] 内连接
来源：http://sl.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gm.9csxet.cn

[Q36] 左连接
来源：http://vh.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kc.newstarts.cn

[Q37] 右连接
来源：http://no.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fl.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xk.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kh.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://gh.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ye.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qy.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tn.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xu.colortex.cn

[Q41] 多表连接
来源：http://rm.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iv.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://wn.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://pe.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://pe.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://pu.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mk.shtwfgs.cn

[Q43] 标量子查询
来源：http://mw.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://we.jctech888.com.cn

[Q44] IN 子查询
来源：http://un.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://gt.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wm.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wf.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ak.panjiajie.cn

[Q47] 与平均值比较
来源：http://ps.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ca.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://ef.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wh.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://rt.jctech888.com.cn

[Q49] 更新单行
来源：http://uy.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ue.asd995.cn

[Q50] 批量更新
来源：http://ny.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://su.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://ey.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ve.chemitech.net.cn

[Q52] 删除指定行
来源：http://yi.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://mm.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://lz.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hm.bookmarksfly.cn

[Q54] 清空表
来源：http://no.newstarts.cn

TRUNCATE TABLE logs;
来源：http://qv.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://st.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://at.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://xi.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tj.hahajie.cn

[Q57] 行号
来源：http://ye.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iw.9csxet.cn

[Q58] 累计求和
来源：http://ec.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cn.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://yg.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sm.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://nw.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vc.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vz.9csxet.cn

[Q61] 移动平均
来源：http://la.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xv.hahajie.cn

[Q62] 分组占比
来源：http://sr.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kp.szxytkj.cn

[Q63] 开启事务
来源：http://rn.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wh.9csxet.cn

[Q64] 提交事务
来源：http://cq.chemitech.net.cn

COMMIT;
来源：http://zz.szsharing.cn

[Q65] 回滚事务
来源：http://me.szsharing.cn

ROLLBACK;
来源：http://ay.nicolike.cn

[Q66] 行锁查询
来源：http://cp.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hy.asd995.cn

[Q67] 设置隔离级别
来源：http://am.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ko.lnxyls.cn

[Q68] 保存点
来源：http://hl.jctech888.com.cn

SAVEPOINT sp1;
来源：http://ee.hahajie.cn

ROLLBACK TO sp1;
来源：http://ne.chemitech.net.cn

[Q69] 查看执行计划
来源：http://cr.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hg.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://py.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://fq.521024.cn

[Q71] 查看建表语句
来源：http://gq.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sc.yuexingan06.cn

[Q72] 查看索引
来源：http://xh.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://bx.huixiangedu.cn

[Q73] 查看表状态
来源：http://po.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xy.hahajie.cn

[Q74] 强制使用索引
来源：http://tg.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zn.wgjwhj.cn

[Q75] 日期格式化
来源：http://ka.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qc.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hr.nszjky.cn

[Q76] 按天统计
来源：http://xm.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yi.hnjuh.cn

[Q77] 时间加减
来源：http://em.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eq.hahajie.cn

[Q78] 当前时间
来源：http://qc.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://io.chemitech.net.cn

[Q79] 字符串拼接
来源：http://qt.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://an.haigaiapp.cn

[Q80] 字符串截取
来源：http://uh.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tu.shxzskj.cn

[Q81] 字符串替换
来源：http://va.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ig.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://zf.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fg.chemitech.net.cn

[Q83] 大小写转换
来源：http://gm.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rf.nicolike.cn

[Q84] 去除首尾空格
来源：http://xe.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://cr.shtwfgs.cn

[Q85] 数值取整
来源：http://kf.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gk.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://iv.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ov.szsharing.cn

[Q87] JSON 字段做条件
来源：http://cr.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://az.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://hl.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sv.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ao.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://ak.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://we.asd995.cn

[Q90] 生成序号列
来源：http://kv.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://is.nszjky.cn

================================================================================
来源：http://us.bookmarksfly.cn

R. Bash 专题
来源：http://ps.jianghongdianzi.cn

================================================================================
来源：http://jx.nicolike.cn

[R01] shebang 与严格模式
来源：http://co.panjiajie.cn

#!/usr/bin/env bash
来源：http://nl.gzmigu.cn

set -euo pipefail
来源：http://ch.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://ce.9csxet.cn

name="Tom"; echo "$name"
来源：http://ij.521024.cn

[R03] 只读变量
来源：http://bh.newstarts.cn

readonly PI=3.14
来源：http://wt.hnjuh.cn

[R04] 位置参数
来源：http://zm.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dg.shtwfgs.cn

[R05] 参数默认值
来源：http://ns.gzmigu.cn

name="${1:-default}"
来源：http://xe.9csxet.cn

[R06] 判断命令是否存在
来源：http://lt.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ea.huixiangedu.cn

[R07] if 判断文件
来源：http://bu.nszjky.cn


<!-- 参考信息 -->