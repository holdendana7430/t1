代发 wailian999

TS:   crypto.randomUUID()
来源：http://eu.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://ku.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://ej.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://xa.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://jw.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://gj.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oi.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oe.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dq.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jr.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tu.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hp.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qg.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lt.hnjuh.cn

[P03] 生成短随机字符串
来源：http://nt.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ss.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mh.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tr.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xs.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bj.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ta.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xc.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://da.huanxung.cn

[P04] 求长度
来源：http://jf.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ix.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://co.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ta.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qy.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://zm.hahajie.cn

Go:   len(arr);  len(m)
来源：http://nd.521024.cn

Ruby: x.length;  x.size
来源：http://ul.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ka.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://ez.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yc.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ao.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aa.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ri.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jl.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hx.huanxung.cn

Ruby: a == b
来源：http://wd.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kx.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fe.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yf.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://gr.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vd.bjjhwx.cn

TS:   if (x == null) {}
来源：http://un.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sf.szxytkj.cn

Go:   if x == nil {}
来源：http://sm.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ch.wgjwhj.cn

C#:   if (x is null) {}
来源：http://ej.521024.cn

[P07] 防抖与节流
来源：http://tl.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sd.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://hp.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xs.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zy.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jr.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hh.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fa.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://dv.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://va.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vj.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tq.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ax.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wo.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ig.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dc.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vp.colortex.cn

================================================================================
来源：http://rk.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://da.gzmigu.cn

================================================================================
来源：http://wr.szsharing.cn

[Q01] 创建表
来源：http://as.haigaiapp.cn

CREATE TABLE users (
来源：http://xl.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ig.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://tu.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://it.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ao.521024.cn

);
来源：http://to.gzmigu.cn

[Q02] 创建带外键的表
来源：http://kl.521024.cn

CREATE TABLE orders (
来源：http://uo.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zf.shtwfgs.cn

user_id INT NOT NULL,
来源：http://fk.asd995.cn

amount DECIMAL(10, 2),
来源：http://bl.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ab.szsharing.cn

);
来源：http://ey.chemitech.net.cn

[Q03] 增加列
来源：http://fc.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://os.newstarts.cn

[Q04] 修改列类型
来源：http://ad.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bp.gzmigu.cn

[Q05] 重命名列
来源：http://uz.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rx.lnxyls.cn

[Q06] 删除列
来源：http://lt.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xz.nszjky.cn

[Q07] 删除表
来源：http://dn.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://ff.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ny.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rp.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://sv.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bm.haigaiapp.cn

[Q10] 插入单行
来源：http://sp.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ta.wgjwhj.cn

[Q11] 一次插入多行
来源：http://uh.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qt.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://gg.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ty.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zj.huanxung.cn

[Q13] 忽略重复插入
来源：http://tk.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qm.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://ok.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jy.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dy.huixinmuqiang.cn

[Q15] 查询全部
来源：http://yj.panjiajie.cn

SELECT * FROM users;
来源：http://gq.nszjky.cn

[Q16] 查询指定列
来源：http://sj.9csxet.cn

SELECT id, name FROM users;
来源：http://ph.bookmarksfly.cn

[Q17] 条件查询
来源：http://ak.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bv.panjiajie.cn

[Q18] 模糊匹配
来源：http://cn.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://st.muxihuayi.cn

[Q19] 范围查询
来源：http://jy.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dj.nicolike.cn

[Q20] IN 列表
来源：http://qc.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hc.521024.cn

[Q21] 空值判断
来源：http://pk.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jo.haigaiapp.cn

[Q22] 排序
来源：http://ph.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ny.hnjuh.cn

[Q23] 分页
来源：http://rt.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nm.bookmarksfly.cn

[Q24] 去重
来源：http://sj.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://eg.szxytkj.cn

[Q25] 只取前 N 条
来源：http://kx.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tb.huixinmuqiang.cn

[Q26] 计数
来源：http://xt.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://ma.shxzukj.cn

[Q27] 条件计数
来源：http://hs.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cp.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://gv.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rn.nicolike.cn

[Q29] 最大最小值
来源：http://qn.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ib.colortex.cn

[Q30] 分组统计
来源：http://hq.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yk.newstarts.cn

[Q31] 分组后过滤
来源：http://yx.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://or.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://hg.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zl.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://de.chemitech.net.cn

[Q33] 多列分组
来源：http://ec.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lp.huanxung.cn

[Q34] 每组取第一条
来源：http://xk.gzmigu.cn

SELECT * FROM (
来源：http://ys.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tn.jctech888.com.cn

) t WHERE rn = 1;
来源：http://nk.hahajie.cn

[Q35] 内连接
来源：http://ku.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bj.panjiajie.cn

[Q36] 左连接
来源：http://oe.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mr.asd995.cn

[Q37] 右连接
来源：http://ii.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kd.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xp.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lq.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://mw.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ds.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iu.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ws.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jo.hnjuh.cn

[Q41] 多表连接
来源：http://gs.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iy.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://kz.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://nz.colortex.cn

[Q42] 连接条件附加过滤
来源：http://av.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://sx.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dg.huanxung.cn

[Q43] 标量子查询
来源：http://ke.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://um.nicolike.cn

[Q44] IN 子查询
来源：http://lp.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fu.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://nl.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ub.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://im.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fi.shxzskj.cn

[Q47] 与平均值比较
来源：http://fz.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tx.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://xz.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ds.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ok.huixinmuqiang.cn

[Q49] 更新单行
来源：http://ce.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nj.bjjhwx.cn

[Q50] 批量更新
来源：http://je.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bn.shtwfgs.cn

[Q51] 用子查询更新
来源：http://zm.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vt.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://os.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://oy.9csxet.cn

[Q53] 按条件删除
来源：http://pd.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ta.colortex.cn

[Q54] 清空表
来源：http://bo.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://ya.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://uq.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wl.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://af.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dt.shxzskj.cn

[Q57] 行号
来源：http://uk.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xq.nicolike.cn

[Q58] 累计求和
来源：http://ih.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cx.muxihuayi.cn

[Q59] 分组内累计
来源：http://xa.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wc.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://dv.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kq.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jh.jianghongdianzi.cn

[Q61] 移动平均
来源：http://wr.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://br.haigaiapp.cn

[Q62] 分组占比
来源：http://xa.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ub.newstarts.cn

[Q63] 开启事务
来源：http://oj.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ew.huixiangedu.cn

[Q64] 提交事务
来源：http://xs.lnxyls.cn

COMMIT;
来源：http://xp.lnxyls.cn

[Q65] 回滚事务
来源：http://do.hnjuh.cn

ROLLBACK;
来源：http://xi.521024.cn

[Q66] 行锁查询
来源：http://lf.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://as.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://tp.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rk.hahajie.cn

[Q68] 保存点
来源：http://rr.hnjuh.cn

SAVEPOINT sp1;
来源：http://nk.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://yl.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://xb.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sn.szxytkj.cn

[Q70] 更新统计信息
来源：http://fo.haigaiapp.cn

ANALYZE TABLE users;
来源：http://yf.szsharing.cn

[Q71] 查看建表语句
来源：http://kt.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xl.huixinmuqiang.cn

[Q72] 查看索引
来源：http://ax.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://zl.bjjhwx.cn

[Q73] 查看表状态
来源：http://xp.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jx.wgjwhj.cn

[Q74] 强制使用索引
来源：http://hr.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dp.szxytkj.cn

[Q75] 日期格式化
来源：http://jc.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zw.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kg.gzmigu.cn

[Q76] 按天统计
来源：http://cm.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oq.9csxet.cn

[Q77] 时间加减
来源：http://ft.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xi.hnjuh.cn

[Q78] 当前时间
来源：http://kr.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ee.muxihuayi.cn

[Q79] 字符串拼接
来源：http://kw.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://or.haigaiapp.cn

[Q80] 字符串截取
来源：http://hq.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kf.chemitech.net.cn

[Q81] 字符串替换
来源：http://bn.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sw.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://nl.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ox.colortex.cn

[Q83] 大小写转换
来源：http://go.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ke.lnxyls.cn

[Q84] 去除首尾空格
来源：http://ca.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://il.newstarts.cn

[Q85] 数值取整
来源：http://zb.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ie.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://es.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dm.nszjky.cn

[Q87] JSON 字段做条件
来源：http://nq.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vg.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://ij.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wy.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xf.lnxyls.cn

[Q89] 判断表是否存在
来源：http://tv.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uv.colortex.cn

[Q90] 生成序号列
来源：http://dc.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cp.huixinmuqiang.cn

================================================================================
来源：http://vy.jctech888.com.cn

R. Bash 专题
来源：http://dt.shxzskj.cn

================================================================================
来源：http://ss.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://yy.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://om.colortex.cn

set -euo pipefail
来源：http://fo.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://si.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://yp.9csxet.cn

[R03] 只读变量
来源：http://iu.bjjhwx.cn

readonly PI=3.14
来源：http://hq.szxytkj.cn

[R04] 位置参数
来源：http://cf.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lw.szsharing.cn

[R05] 参数默认值
来源：http://pb.lnxyls.cn

name="${1:-default}"
来源：http://gu.lnxyls.cn

[R06] 判断命令是否存在
来源：http://ne.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ov.wgjwhj.cn

[R07] if 判断文件
来源：http://ej.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tv.bjjhwx.cn

[R08] 数值比较
来源：http://cu.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eq.huanxung.cn

[R09] 字符串比较
来源：http://ls.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rj.jianghongdianzi.cn

[R10] 正则匹配
来源：http://se.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nt.lnxyls.cn

[R11] case 多分支
来源：http://ra.muxihuayi.cn


<!-- 参考信息 -->