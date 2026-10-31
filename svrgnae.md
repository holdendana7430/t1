代发 wailian999

C#:   Parallel.For
来源：http://pl.huixinmuqiang.cn

================================================================================
来源：http://vb.yuexingan06.cn

P. 常用工具函数
来源：http://tw.nicolike.cn

================================================================================
来源：http://iq.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://sf.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://zd.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dx.9csxet.cn

JS:   crypto.randomUUID()
来源：http://hw.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://gc.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://se.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://rn.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://ku.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://rj.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://qa.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sc.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://me.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vc.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oj.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://px.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ky.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gj.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fs.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://ry.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cy.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wx.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vm.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qb.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://af.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ki.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ji.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sl.shxzskj.cn

[P04] 求长度
来源：http://zx.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mc.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qa.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://al.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ja.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://tx.asd995.cn

Go:   len(arr);  len(m)
来源：http://vs.asd995.cn

Ruby: x.length;  x.size
来源：http://am.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mv.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://jl.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tp.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bq.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kd.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gh.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://en.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rb.szxytkj.cn

Ruby: a == b
来源：http://wx.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nc.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ed.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wd.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://rr.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bu.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ny.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nm.bookmarksfly.cn

Go:   if x == nil {}
来源：http://km.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mr.nicolike.cn

C#:   if (x is null) {}
来源：http://vo.gzmigu.cn

[P07] 防抖与节流
来源：http://wo.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cs.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://la.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rf.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pe.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ew.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hc.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bw.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sc.nszjky.cn

[P08] 处理浮点精度问题
来源：http://gr.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xb.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nh.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://um.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uc.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vo.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yt.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://go.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ie.shxzukj.cn

================================================================================
来源：http://nk.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eu.yuntaijiaju.cn

================================================================================
来源：http://af.muxihuayi.cn

[Q01] 创建表
来源：http://da.newstarts.cn

CREATE TABLE users (
来源：http://em.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vz.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://gn.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://nv.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nf.wgjwhj.cn

);
来源：http://mp.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://fc.gzmigu.cn

CREATE TABLE orders (
来源：http://wx.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rb.shtwfgs.cn

user_id INT NOT NULL,
来源：http://ok.hahajie.cn

amount DECIMAL(10, 2),
来源：http://bw.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ya.shxzskj.cn

);
来源：http://ke.panjiajie.cn

[Q03] 增加列
来源：http://ry.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ft.shxzskj.cn

[Q04] 修改列类型
来源：http://ev.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yy.shxzukj.cn

[Q05] 重命名列
来源：http://fl.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fn.panjiajie.cn

[Q06] 删除列
来源：http://kz.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hx.bjjhwx.cn

[Q07] 删除表
来源：http://sk.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://uv.muxihuayi.cn

[Q08] 创建普通索引
来源：http://pn.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://da.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://my.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fs.szxytkj.cn

[Q10] 插入单行
来源：http://pn.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bz.muxihuayi.cn

[Q11] 一次插入多行
来源：http://ja.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bz.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://du.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tu.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rm.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://ta.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mq.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://dq.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wp.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yp.wgjwhj.cn

[Q15] 查询全部
来源：http://ar.hahajie.cn

SELECT * FROM users;
来源：http://dz.bookmarksfly.cn

[Q16] 查询指定列
来源：http://pe.hahajie.cn

SELECT id, name FROM users;
来源：http://qe.hnjuh.cn

[Q17] 条件查询
来源：http://kt.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fz.szxytkj.cn

[Q18] 模糊匹配
来源：http://gv.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dz.huixinmuqiang.cn

[Q19] 范围查询
来源：http://vz.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ok.huixinmuqiang.cn

[Q20] IN 列表
来源：http://rq.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://to.muxihuayi.cn

[Q21] 空值判断
来源：http://xn.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://az.muxihuayi.cn

[Q22] 排序
来源：http://wx.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nm.gzmigu.cn

[Q23] 分页
来源：http://ak.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wd.nszjky.cn

[Q24] 去重
来源：http://df.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://wg.asd995.cn

[Q25] 只取前 N 条
来源：http://gy.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ru.jianghongdianzi.cn

[Q26] 计数
来源：http://hw.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ix.yuexingan06.cn

[Q27] 条件计数
来源：http://eo.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kg.9csxet.cn

[Q28] 求和与平均
来源：http://gr.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bk.lnxyls.cn

[Q29] 最大最小值
来源：http://qh.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cv.hahajie.cn

[Q30] 分组统计
来源：http://ev.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vh.chemitech.net.cn

[Q31] 分组后过滤
来源：http://qa.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bv.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://ls.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ln.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tm.521024.cn

[Q33] 多列分组
来源：http://sm.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fb.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://pn.bjjhwx.cn

SELECT * FROM (
来源：http://af.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://js.nszjky.cn

) t WHERE rn = 1;
来源：http://lu.huixiangedu.cn

[Q35] 内连接
来源：http://hw.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qm.nszjky.cn

[Q36] 左连接
来源：http://co.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://el.521024.cn

[Q37] 右连接
来源：http://ee.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ba.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cn.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ub.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ma.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ve.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dj.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ib.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lo.gzmigu.cn

[Q41] 多表连接
来源：http://qy.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://go.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://de.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://fl.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://yb.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://tr.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dw.yuexingan06.cn

[Q43] 标量子查询
来源：http://ua.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xx.haigaiapp.cn

[Q44] IN 子查询
来源：http://jy.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ka.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://dz.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xt.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yx.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://az.hahajie.cn

[Q47] 与平均值比较
来源：http://dg.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rl.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://ir.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yk.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://dy.shtwfgs.cn

[Q49] 更新单行
来源：http://of.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qm.lnxyls.cn

[Q50] 批量更新
来源：http://oi.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cd.colortex.cn

[Q51] 用子查询更新
来源：http://at.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pr.shtwfgs.cn

[Q52] 删除指定行
来源：http://iy.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://ga.bookmarksfly.cn

[Q53] 按条件删除
来源：http://ux.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pg.chemitech.net.cn

[Q54] 清空表
来源：http://tz.521024.cn

TRUNCATE TABLE logs;
来源：http://ry.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://zz.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vh.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://rt.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nm.asd995.cn

[Q57] 行号
来源：http://tw.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bd.lnxyls.cn

[Q58] 累计求和
来源：http://fm.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sd.jctech888.com.cn

[Q59] 分组内累计
来源：http://bm.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vh.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://bf.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bi.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uz.szsharing.cn

[Q61] 移动平均
来源：http://dq.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ug.szxytkj.cn

[Q62] 分组占比
来源：http://ke.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cz.hahajie.cn

[Q63] 开启事务
来源：http://kp.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://co.9csxet.cn

[Q64] 提交事务
来源：http://lc.huanxung.cn

COMMIT;
来源：http://rz.9csxet.cn

[Q65] 回滚事务
来源：http://dn.huanxung.cn

ROLLBACK;
来源：http://wg.colortex.cn

[Q66] 行锁查询
来源：http://mo.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ce.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://wp.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dx.szsharing.cn

[Q68] 保存点
来源：http://bb.huanxung.cn

SAVEPOINT sp1;
来源：http://wi.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://kb.bjjhwx.cn

[Q69] 查看执行计划
来源：http://bz.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zw.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://vc.shxzukj.cn

ANALYZE TABLE users;
来源：http://iy.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://ez.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nf.newstarts.cn

[Q72] 查看索引
来源：http://hc.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://ev.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://bm.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pe.nicolike.cn

[Q74] 强制使用索引
来源：http://nc.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sf.yuexingan06.cn

[Q75] 日期格式化
来源：http://pi.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vm.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wh.shxzukj.cn

[Q76] 按天统计
来源：http://cz.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wt.asd995.cn

[Q77] 时间加减
来源：http://mv.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bl.bookmarksfly.cn

[Q78] 当前时间
来源：http://wn.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bn.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://ob.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ov.jctech888.com.cn

[Q80] 字符串截取
来源：http://to.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vv.nszjky.cn

[Q81] 字符串替换
来源：http://sr.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ko.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://ji.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pm.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://wd.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://si.hahajie.cn

[Q84] 去除首尾空格
来源：http://kp.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://rv.newstarts.cn

[Q85] 数值取整
来源：http://ev.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fi.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://mt.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jv.newstarts.cn

[Q87] JSON 字段做条件
来源：http://vp.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://is.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://ny.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ek.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dd.huanxung.cn

[Q89] 判断表是否存在
来源：http://pn.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pb.yuexingan06.cn

[Q90] 生成序号列
来源：http://ru.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iv.wgjwhj.cn

================================================================================
来源：http://mp.chemitech.net.cn

R. Bash 专题
来源：http://ed.jianghongdianzi.cn

================================================================================
来源：http://ay.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://vc.szsharing.cn

#!/usr/bin/env bash
来源：http://hv.shtwfgs.cn

set -euo pipefail
来源：http://ta.521024.cn

[R02] 变量赋值与使用
来源：http://ic.hahajie.cn

name="Tom"; echo "$name"
来源：http://eo.jctech888.com.cn

[R03] 只读变量
来源：http://dx.nicolike.cn

readonly PI=3.14
来源：http://ek.shtwfgs.cn

[R04] 位置参数
来源：http://od.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aj.huixinmuqiang.cn

[R05] 参数默认值
来源：http://zw.shxzukj.cn

name="${1:-default}"
来源：http://qg.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://pv.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hj.hnjuh.cn

[R07] if 判断文件
来源：http://eu.lnxyls.cn


<!-- 参考信息 -->