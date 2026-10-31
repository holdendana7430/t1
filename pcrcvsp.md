代发 wailian999

C#:   Parallel.For
来源：http://cy.colortex.cn

================================================================================
来源：http://hs.haigaiapp.cn

P. 常用工具函数
来源：http://jg.szxytkj.cn

================================================================================
来源：http://bk.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://vj.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://ap.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fv.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://ma.colortex.cn

TS:   crypto.randomUUID()
来源：http://th.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://aa.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://et.521024.cn

Ruby: SecureRandom.uuid
来源：http://ma.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://xq.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://tg.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rs.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wx.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mb.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eb.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uz.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ma.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jt.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yc.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://hq.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ka.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dy.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ok.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xp.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kf.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qb.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sr.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://by.jianghongdianzi.cn

[P04] 求长度
来源：http://wx.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uc.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zr.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://an.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lc.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://ch.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://vk.nszjky.cn

Ruby: x.length;  x.size
来源：http://sd.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ay.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://kt.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://za.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nt.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ak.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://af.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mo.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://il.haigaiapp.cn

Ruby: a == b
来源：http://jc.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zy.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ez.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nd.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://ms.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dh.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ns.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cq.colortex.cn

Go:   if x == nil {}
来源：http://ul.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mw.hahajie.cn

C#:   if (x is null) {}
来源：http://il.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://ic.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kv.521024.cn

PHP:  // 手写时间戳比较
来源：http://ui.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cm.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bb.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ne.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sx.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xj.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://no.nszjky.cn

[P08] 处理浮点精度问题
来源：http://nk.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gb.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hn.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bb.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zw.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cd.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kw.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://op.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sy.bjjhwx.cn

================================================================================
来源：http://gs.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dy.panjiajie.cn

================================================================================
来源：http://pp.nicolike.cn

[Q01] 创建表
来源：http://oa.9csxet.cn

CREATE TABLE users (
来源：http://xw.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ok.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://vr.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://uf.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bu.shxzskj.cn

);
来源：http://jt.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://xt.nszjky.cn

CREATE TABLE orders (
来源：http://wv.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ac.panjiajie.cn

user_id INT NOT NULL,
来源：http://dq.9csxet.cn

amount DECIMAL(10, 2),
来源：http://fa.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pw.nicolike.cn

);
来源：http://ws.huixinmuqiang.cn

[Q03] 增加列
来源：http://hj.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zm.521024.cn

[Q04] 修改列类型
来源：http://ks.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jf.bookmarksfly.cn

[Q05] 重命名列
来源：http://rc.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fc.huixiangedu.cn

[Q06] 删除列
来源：http://oi.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ls.shxzskj.cn

[Q07] 删除表
来源：http://ke.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://xd.lnxyls.cn

[Q08] 创建普通索引
来源：http://yt.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sd.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://ev.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wx.jianghongdianzi.cn

[Q10] 插入单行
来源：http://zg.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cr.huanxung.cn

[Q11] 一次插入多行
来源：http://km.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wv.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://rn.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zm.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uw.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://vf.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uy.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://jg.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vy.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zn.muxihuayi.cn

[Q15] 查询全部
来源：http://yv.panjiajie.cn

SELECT * FROM users;
来源：http://sm.shxzskj.cn

[Q16] 查询指定列
来源：http://yq.nszjky.cn

SELECT id, name FROM users;
来源：http://db.haigaiapp.cn

[Q17] 条件查询
来源：http://vj.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ia.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://cl.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xm.bjjhwx.cn

[Q19] 范围查询
来源：http://iw.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fa.szxytkj.cn

[Q20] IN 列表
来源：http://bf.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xn.gzmigu.cn

[Q21] 空值判断
来源：http://xd.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fd.jctech888.com.cn

[Q22] 排序
来源：http://st.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tw.szxytkj.cn

[Q23] 分页
来源：http://fd.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kw.newstarts.cn

[Q24] 去重
来源：http://yz.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://pp.huanxung.cn

[Q25] 只取前 N 条
来源：http://rx.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ai.newstarts.cn

[Q26] 计数
来源：http://if.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://tv.asd995.cn

[Q27] 条件计数
来源：http://gj.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hv.nszjky.cn

[Q28] 求和与平均
来源：http://yi.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jf.huixiangedu.cn

[Q29] 最大最小值
来源：http://zy.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vq.nicolike.cn

[Q30] 分组统计
来源：http://dn.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://td.szsharing.cn

[Q31] 分组后过滤
来源：http://bw.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jo.newstarts.cn

[Q32] 分组拼接字符串
来源：http://kj.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yp.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gi.lnxyls.cn

[Q33] 多列分组
来源：http://ep.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wu.shxzukj.cn

[Q34] 每组取第一条
来源：http://gq.yuexingan06.cn

SELECT * FROM (
来源：http://av.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tc.521024.cn

) t WHERE rn = 1;
来源：http://jq.jctech888.com.cn

[Q35] 内连接
来源：http://za.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jp.lnxyls.cn

[Q36] 左连接
来源：http://gy.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xv.bjjhwx.cn

[Q37] 右连接
来源：http://ev.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ny.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bq.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fs.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://mt.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ld.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ul.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hl.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lu.huanxung.cn

[Q41] 多表连接
来源：http://cv.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fd.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://uz.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://fn.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://sn.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://zy.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tb.wgjwhj.cn

[Q43] 标量子查询
来源：http://am.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rf.asd995.cn

[Q44] IN 子查询
来源：http://ox.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xc.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://ri.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pe.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ss.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hn.lnxyls.cn

[Q47] 与平均值比较
来源：http://jl.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://af.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ay.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cn.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://zm.nszjky.cn

[Q49] 更新单行
来源：http://im.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gp.chemitech.net.cn

[Q50] 批量更新
来源：http://oh.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ik.shtwfgs.cn

[Q51] 用子查询更新
来源：http://pt.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mo.asd995.cn

[Q52] 删除指定行
来源：http://rx.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://wv.nicolike.cn

[Q53] 按条件删除
来源：http://nu.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ha.shxzukj.cn

[Q54] 清空表
来源：http://gv.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://je.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://cu.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ms.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://jp.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ik.521024.cn

[Q57] 行号
来源：http://ng.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lt.bookmarksfly.cn

[Q58] 累计求和
来源：http://jx.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ry.colortex.cn

[Q59] 分组内累计
来源：http://oj.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lu.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://wa.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cv.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://if.newstarts.cn

[Q61] 移动平均
来源：http://ru.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ek.chemitech.net.cn

[Q62] 分组占比
来源：http://jz.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jj.gzmigu.cn

[Q63] 开启事务
来源：http://qh.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ht.nszjky.cn

[Q64] 提交事务
来源：http://bn.bjjhwx.cn

COMMIT;
来源：http://di.panjiajie.cn

[Q65] 回滚事务
来源：http://vu.huixinmuqiang.cn

ROLLBACK;
来源：http://kq.wgjwhj.cn

[Q66] 行锁查询
来源：http://tr.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://de.9csxet.cn

[Q67] 设置隔离级别
来源：http://uz.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sa.asd995.cn

[Q68] 保存点
来源：http://bm.gzmigu.cn

SAVEPOINT sp1;
来源：http://mx.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://gk.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://op.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hi.panjiajie.cn

[Q70] 更新统计信息
来源：http://ol.asd995.cn

ANALYZE TABLE users;
来源：http://rl.gzmigu.cn

[Q71] 查看建表语句
来源：http://el.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vg.shxzskj.cn

[Q72] 查看索引
来源：http://ew.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://oi.shxzukj.cn

[Q73] 查看表状态
来源：http://so.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ey.colortex.cn

[Q74] 强制使用索引
来源：http://xh.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ay.panjiajie.cn

[Q75] 日期格式化
来源：http://wl.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nm.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ue.huanxung.cn

[Q76] 按天统计
来源：http://iv.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rc.gzmigu.cn

[Q77] 时间加减
来源：http://cv.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qi.bookmarksfly.cn

[Q78] 当前时间
来源：http://fb.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aa.colortex.cn

[Q79] 字符串拼接
来源：http://vj.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lh.huixiangedu.cn

[Q80] 字符串截取
来源：http://mp.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hp.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://wb.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ng.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://mw.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gr.yuexingan06.cn

[Q83] 大小写转换
来源：http://hx.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oe.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://oo.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://ca.yuexingan06.cn

[Q85] 数值取整
来源：http://fp.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://np.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://rx.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rn.nicolike.cn

[Q87] JSON 字段做条件
来源：http://hp.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iy.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://ad.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://js.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://md.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://hj.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sr.colortex.cn

[Q90] 生成序号列
来源：http://ml.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wg.gzmigu.cn

================================================================================
来源：http://wb.shxzskj.cn

R. Bash 专题
来源：http://wy.yuexingan06.cn

================================================================================
来源：http://kw.shxzukj.cn

[R01] shebang 与严格模式
来源：http://wo.panjiajie.cn

#!/usr/bin/env bash
来源：http://pe.colortex.cn

set -euo pipefail
来源：http://so.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://uz.colortex.cn

name="Tom"; echo "$name"
来源：http://om.szsharing.cn

[R03] 只读变量
来源：http://no.chemitech.net.cn

readonly PI=3.14
来源：http://ga.jctech888.com.cn

[R04] 位置参数
来源：http://nx.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uu.9csxet.cn

[R05] 参数默认值
来源：http://xu.colortex.cn

name="${1:-default}"
来源：http://ie.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://wc.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gb.hnjuh.cn

[R07] if 判断文件
来源：http://mk.huixinmuqiang.cn


<!-- 参考信息 -->