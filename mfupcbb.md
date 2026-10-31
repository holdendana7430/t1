代发 wailian999

[P01] 生成 UUID
来源：http://rv.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://bd.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ym.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://az.huanxung.cn

TS:   crypto.randomUUID()
来源：http://on.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://lz.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://lj.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://or.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://kt.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://am.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kp.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qa.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zz.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hq.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yg.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vl.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cv.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bt.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://hv.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://us.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sa.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qn.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xz.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qv.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lw.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xw.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ad.huanxung.cn

[P04] 求长度
来源：http://sc.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bb.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dt.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bf.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ba.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://kr.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://gy.shxzukj.cn

Ruby: x.length;  x.size
来源：http://gz.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lq.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://qg.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ig.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nz.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cf.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ih.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gz.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ao.521024.cn

Ruby: a == b
来源：http://tp.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ja.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hg.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hs.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://xz.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gn.9csxet.cn

TS:   if (x == null) {}
来源：http://zy.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cu.bjjhwx.cn

Go:   if x == nil {}
来源：http://ya.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ea.hnjuh.cn

C#:   if (x is null) {}
来源：http://pt.lnxyls.cn

[P07] 防抖与节流
来源：http://qp.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gt.asd995.cn

PHP:  // 手写时间戳比较
来源：http://ws.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ph.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nt.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zl.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fd.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://va.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fy.nicolike.cn

[P08] 处理浮点精度问题
来源：http://jp.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kn.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gl.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dg.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kp.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yi.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yn.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jq.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mu.jctech888.com.cn

================================================================================
来源：http://de.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ks.bjjhwx.cn

================================================================================
来源：http://tc.haigaiapp.cn

[Q01] 创建表
来源：http://kj.chemitech.net.cn

CREATE TABLE users (
来源：http://lc.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pg.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://xl.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://di.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ft.521024.cn

);
来源：http://zw.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://cg.shtwfgs.cn

CREATE TABLE orders (
来源：http://tx.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qj.chemitech.net.cn

user_id INT NOT NULL,
来源：http://mk.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://gg.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rb.hnjuh.cn

);
来源：http://sp.colortex.cn

[Q03] 增加列
来源：http://kz.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ls.huixiangedu.cn

[Q04] 修改列类型
来源：http://zr.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fe.muxihuayi.cn

[Q05] 重命名列
来源：http://ed.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kb.jianghongdianzi.cn

[Q06] 删除列
来源：http://wc.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ex.wgjwhj.cn

[Q07] 删除表
来源：http://tr.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://ng.panjiajie.cn

[Q08] 创建普通索引
来源：http://jd.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xc.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://qh.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ch.yuexingan06.cn

[Q10] 插入单行
来源：http://qi.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hb.wgjwhj.cn

[Q11] 一次插入多行
来源：http://hb.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xs.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ue.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xz.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ji.lnxyls.cn

[Q13] 忽略重复插入
来源：http://lj.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://en.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://oj.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zw.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zp.yuntaijiaju.cn

[Q15] 查询全部
来源：http://tb.lnxyls.cn

SELECT * FROM users;
来源：http://vy.nicolike.cn

[Q16] 查询指定列
来源：http://rb.muxihuayi.cn

SELECT id, name FROM users;
来源：http://cb.szxytkj.cn

[Q17] 条件查询
来源：http://vk.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lt.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://gz.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cm.chemitech.net.cn

[Q19] 范围查询
来源：http://cc.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ju.shxzskj.cn

[Q20] IN 列表
来源：http://gq.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://go.yuexingan06.cn

[Q21] 空值判断
来源：http://it.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nw.nicolike.cn

[Q22] 排序
来源：http://qz.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pg.haigaiapp.cn

[Q23] 分页
来源：http://eh.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pt.yuntaijiaju.cn

[Q24] 去重
来源：http://ay.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://li.hnjuh.cn

[Q25] 只取前 N 条
来源：http://cj.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pb.bookmarksfly.cn

[Q26] 计数
来源：http://fk.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://iv.yuntaijiaju.cn

[Q27] 条件计数
来源：http://yv.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fy.haigaiapp.cn

[Q28] 求和与平均
来源：http://xc.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dw.521024.cn

[Q29] 最大最小值
来源：http://zu.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cw.jianghongdianzi.cn

[Q30] 分组统计
来源：http://uf.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://to.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ed.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eb.521024.cn

[Q32] 分组拼接字符串
来源：http://mr.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://po.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qc.wgjwhj.cn

[Q33] 多列分组
来源：http://ak.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zy.hahajie.cn

[Q34] 每组取第一条
来源：http://bk.huixinmuqiang.cn

SELECT * FROM (
来源：http://be.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iq.bjjhwx.cn

) t WHERE rn = 1;
来源：http://yt.lnxyls.cn

[Q35] 内连接
来源：http://xe.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://op.hahajie.cn

[Q36] 左连接
来源：http://we.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://us.muxihuayi.cn

[Q37] 右连接
来源：http://md.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ib.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lk.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ub.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://uc.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jp.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nf.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wo.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qg.yuexingan06.cn

[Q41] 多表连接
来源：http://oo.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ms.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://cx.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://mb.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://pi.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://lz.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zk.shtwfgs.cn

[Q43] 标量子查询
来源：http://yv.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dk.haigaiapp.cn

[Q44] IN 子查询
来源：http://cl.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wj.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://mk.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lp.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wx.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iu.gzmigu.cn

[Q47] 与平均值比较
来源：http://xv.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bp.521024.cn

[Q48] CTE 公用表表达式
来源：http://yk.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://by.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://bw.nszjky.cn

[Q49] 更新单行
来源：http://nw.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rv.shxzukj.cn

[Q50] 批量更新
来源：http://yj.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sa.yuexingan06.cn

[Q51] 用子查询更新
来源：http://pt.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wq.shtwfgs.cn

[Q52] 删除指定行
来源：http://mt.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://gi.muxihuayi.cn

[Q53] 按条件删除
来源：http://ct.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://il.bjjhwx.cn

[Q54] 清空表
来源：http://pn.hahajie.cn

TRUNCATE TABLE logs;
来源：http://zj.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://xk.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ch.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://cw.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ms.jianghongdianzi.cn

[Q57] 行号
来源：http://zk.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pw.lnxyls.cn

[Q58] 累计求和
来源：http://nm.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rm.bookmarksfly.cn

[Q59] 分组内累计
来源：http://mx.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mn.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://lp.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bu.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://co.shtwfgs.cn

[Q61] 移动平均
来源：http://hx.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ec.gzmigu.cn

[Q62] 分组占比
来源：http://xk.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ic.wgjwhj.cn

[Q63] 开启事务
来源：http://dq.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ne.yuntaijiaju.cn

[Q64] 提交事务
来源：http://gy.newstarts.cn

COMMIT;
来源：http://uo.shxzukj.cn

[Q65] 回滚事务
来源：http://vq.shtwfgs.cn

ROLLBACK;
来源：http://yh.lnxyls.cn

[Q66] 行锁查询
来源：http://py.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ar.nszjky.cn

[Q67] 设置隔离级别
来源：http://ms.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bo.hahajie.cn

[Q68] 保存点
来源：http://ij.nszjky.cn

SAVEPOINT sp1;
来源：http://bu.9csxet.cn

ROLLBACK TO sp1;
来源：http://ge.szsharing.cn

[Q69] 查看执行计划
来源：http://do.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://im.yuexingan06.cn

[Q70] 更新统计信息
来源：http://ln.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://fi.panjiajie.cn

[Q71] 查看建表语句
来源：http://rt.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://po.szxytkj.cn

[Q72] 查看索引
来源：http://jy.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://ft.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://tw.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bj.muxihuayi.cn

[Q74] 强制使用索引
来源：http://xo.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xk.9csxet.cn

[Q75] 日期格式化
来源：http://xy.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sm.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bj.haigaiapp.cn

[Q76] 按天统计
来源：http://et.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dm.newstarts.cn

[Q77] 时间加减
来源：http://du.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ug.521024.cn

[Q78] 当前时间
来源：http://nx.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ub.jctech888.com.cn

[Q79] 字符串拼接
来源：http://gn.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xo.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://nv.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rz.bjjhwx.cn

[Q81] 字符串替换
来源：http://ze.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bg.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://ih.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nw.nszjky.cn

[Q83] 大小写转换
来源：http://gy.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://it.gzmigu.cn

[Q84] 去除首尾空格
来源：http://ui.521024.cn

SELECT TRIM(name) FROM users;
来源：http://in.hnjuh.cn

[Q85] 数值取整
来源：http://hj.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ke.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://ri.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ez.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://nz.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bq.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://aw.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sz.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ss.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://ti.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qu.haigaiapp.cn

[Q90] 生成序号列
来源：http://go.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rg.newstarts.cn

================================================================================
来源：http://ci.hnjuh.cn

R. Bash 专题
来源：http://jf.lnxyls.cn

================================================================================
来源：http://gy.gzmigu.cn

[R01] shebang 与严格模式
来源：http://ou.wgjwhj.cn

#!/usr/bin/env bash
来源：http://ho.panjiajie.cn

set -euo pipefail
来源：http://qa.huanxung.cn

[R02] 变量赋值与使用
来源：http://mr.nszjky.cn

name="Tom"; echo "$name"
来源：http://sd.lnxyls.cn

[R03] 只读变量
来源：http://zd.asd995.cn

readonly PI=3.14
来源：http://sx.9csxet.cn

[R04] 位置参数
来源：http://ev.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wd.bookmarksfly.cn

[R05] 参数默认值
来源：http://tb.panjiajie.cn

name="${1:-default}"
来源：http://le.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://lx.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hx.9csxet.cn

[R07] if 判断文件
来源：http://nl.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cv.jctech888.com.cn

[R08] 数值比较
来源：http://cb.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pu.yuexingan06.cn

[R09] 字符串比较
来源：http://me.szxytkj.cn


<!-- 参考信息 -->