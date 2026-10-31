代发 wailian999

TS:   crypto.randomUUID()
来源：http://rg.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://vb.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://bc.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://sx.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://bq.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://xu.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oa.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ry.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ru.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wo.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://px.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ij.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xs.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fn.nicolike.cn

[P03] 生成短随机字符串
来源：http://wo.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dh.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ge.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bl.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kj.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://po.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://so.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xq.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://or.colortex.cn

[P04] 求长度
来源：http://yx.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ce.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ti.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://od.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hd.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://as.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://ia.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://dj.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ta.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://sn.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uf.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zg.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ji.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kc.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gj.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ej.asd995.cn

Ruby: a == b
来源：http://nf.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tr.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gx.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nu.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://hd.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ml.szxytkj.cn

TS:   if (x == null) {}
来源：http://qx.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qb.huixiangedu.cn

Go:   if x == nil {}
来源：http://ip.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://di.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://zl.hnjuh.cn

[P07] 防抖与节流
来源：http://lx.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mh.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://ca.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wh.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aw.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kw.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gx.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xc.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://nf.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ch.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ck.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bg.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ud.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nf.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bs.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sd.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bu.szxytkj.cn

================================================================================
来源：http://dc.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nk.huixiangedu.cn

================================================================================
来源：http://hn.shxzskj.cn

[Q01] 创建表
来源：http://ui.yuntaijiaju.cn

CREATE TABLE users (
来源：http://zi.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://av.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://an.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://gk.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ag.lnxyls.cn

);
来源：http://uz.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://sd.shxzukj.cn

CREATE TABLE orders (
来源：http://xe.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fx.chemitech.net.cn

user_id INT NOT NULL,
来源：http://hs.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://aw.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fz.chemitech.net.cn

);
来源：http://kq.panjiajie.cn

[Q03] 增加列
来源：http://aq.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hg.panjiajie.cn

[Q04] 修改列类型
来源：http://aj.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ws.panjiajie.cn

[Q05] 重命名列
来源：http://wv.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cl.yuntaijiaju.cn

[Q06] 删除列
来源：http://cy.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hf.521024.cn

[Q07] 删除表
来源：http://oy.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ld.wgjwhj.cn

[Q08] 创建普通索引
来源：http://xn.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ad.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://hr.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gp.gzmigu.cn

[Q10] 插入单行
来源：http://yu.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ip.hnjuh.cn

[Q11] 一次插入多行
来源：http://um.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tz.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://bz.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jn.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mh.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://sg.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yy.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://px.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hb.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kc.yuntaijiaju.cn

[Q15] 查询全部
来源：http://yn.huixinmuqiang.cn

SELECT * FROM users;
来源：http://vj.bjjhwx.cn

[Q16] 查询指定列
来源：http://oi.gzmigu.cn

SELECT id, name FROM users;
来源：http://yp.asd995.cn

[Q17] 条件查询
来源：http://ye.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jt.shxzukj.cn

[Q18] 模糊匹配
来源：http://mi.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ar.asd995.cn

[Q19] 范围查询
来源：http://gw.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wn.panjiajie.cn

[Q20] IN 列表
来源：http://dz.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fm.hnjuh.cn

[Q21] 空值判断
来源：http://nz.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ad.chemitech.net.cn

[Q22] 排序
来源：http://wb.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qm.szsharing.cn

[Q23] 分页
来源：http://ms.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gv.newstarts.cn

[Q24] 去重
来源：http://tr.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://yy.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://ty.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ds.yuexingan06.cn

[Q26] 计数
来源：http://ad.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://qf.9csxet.cn

[Q27] 条件计数
来源：http://au.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ze.nicolike.cn

[Q28] 求和与平均
来源：http://tl.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ci.gzmigu.cn

[Q29] 最大最小值
来源：http://lv.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nv.hnjuh.cn

[Q30] 分组统计
来源：http://kw.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vx.huanxung.cn

[Q31] 分组后过滤
来源：http://ie.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://go.hahajie.cn

[Q32] 分组拼接字符串
来源：http://us.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jq.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wq.yuexingan06.cn

[Q33] 多列分组
来源：http://vc.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ve.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://gc.jctech888.com.cn

SELECT * FROM (
来源：http://iw.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zf.szsharing.cn

) t WHERE rn = 1;
来源：http://op.lnxyls.cn

[Q35] 内连接
来源：http://iq.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mu.colortex.cn

[Q36] 左连接
来源：http://fd.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wt.newstarts.cn

[Q37] 右连接
来源：http://oe.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qw.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wh.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qe.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://yo.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aj.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tp.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rk.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wl.lnxyls.cn

[Q41] 多表连接
来源：http://xp.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ad.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://gb.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://of.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://va.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://pn.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fq.lnxyls.cn

[Q43] 标量子查询
来源：http://ax.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://to.colortex.cn

[Q44] IN 子查询
来源：http://pc.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pb.colortex.cn

[Q45] EXISTS 判断存在
来源：http://qh.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vl.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ol.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pq.521024.cn

[Q47] 与平均值比较
来源：http://ky.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wc.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://np.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://do.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://wn.gzmigu.cn

[Q49] 更新单行
来源：http://qn.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fd.yuntaijiaju.cn

[Q50] 批量更新
来源：http://qu.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kz.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://dk.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fh.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://mu.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://ud.chemitech.net.cn

[Q53] 按条件删除
来源：http://ho.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sr.shxzskj.cn

[Q54] 清空表
来源：http://qj.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://we.nicolike.cn

[Q55] 排名（并列占位）
来源：http://he.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bx.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://wi.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nq.shxzukj.cn

[Q57] 行号
来源：http://ym.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ct.huixinmuqiang.cn

[Q58] 累计求和
来源：http://hi.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tp.9csxet.cn

[Q59] 分组内累计
来源：http://vm.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://al.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://ir.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rx.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ke.gzmigu.cn

[Q61] 移动平均
来源：http://sf.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jl.jctech888.com.cn

[Q62] 分组占比
来源：http://nu.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tf.asd995.cn

[Q63] 开启事务
来源：http://li.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dz.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ox.shxzukj.cn

COMMIT;
来源：http://qw.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://le.521024.cn

ROLLBACK;
来源：http://rg.huanxung.cn

[Q66] 行锁查询
来源：http://cp.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hl.hahajie.cn

[Q67] 设置隔离级别
来源：http://jb.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fv.huixiangedu.cn

[Q68] 保存点
来源：http://sa.shxzukj.cn

SAVEPOINT sp1;
来源：http://cf.lnxyls.cn

ROLLBACK TO sp1;
来源：http://yr.nicolike.cn

[Q69] 查看执行计划
来源：http://dw.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pu.shxzukj.cn

[Q70] 更新统计信息
来源：http://qh.chemitech.net.cn

ANALYZE TABLE users;
来源：http://cg.newstarts.cn

[Q71] 查看建表语句
来源：http://kw.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zv.yuexingan06.cn

[Q72] 查看索引
来源：http://iw.asd995.cn

SHOW INDEX FROM users;
来源：http://ni.szxytkj.cn

[Q73] 查看表状态
来源：http://st.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ju.yuexingan06.cn

[Q74] 强制使用索引
来源：http://kf.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://id.wgjwhj.cn

[Q75] 日期格式化
来源：http://hn.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pn.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qz.gzmigu.cn

[Q76] 按天统计
来源：http://gs.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zd.huixiangedu.cn

[Q77] 时间加减
来源：http://ah.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ve.haigaiapp.cn

[Q78] 当前时间
来源：http://ja.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fm.muxihuayi.cn

[Q79] 字符串拼接
来源：http://ke.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mh.shxzukj.cn

[Q80] 字符串截取
来源：http://qx.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dp.wgjwhj.cn

[Q81] 字符串替换
来源：http://ma.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jk.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ah.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pd.jctech888.com.cn

[Q83] 大小写转换
来源：http://mr.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rr.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://gm.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://os.nszjky.cn

[Q85] 数值取整
来源：http://fa.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qk.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://xy.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nl.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://gf.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qn.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://qu.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bl.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ts.nszjky.cn

[Q89] 判断表是否存在
来源：http://fg.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vf.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://qs.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://de.chemitech.net.cn

================================================================================
来源：http://gc.nicolike.cn

R. Bash 专题
来源：http://ds.wgjwhj.cn

================================================================================
来源：http://ps.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://yl.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://sa.gzmigu.cn

set -euo pipefail
来源：http://jw.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://rl.lnxyls.cn

name="Tom"; echo "$name"
来源：http://iw.colortex.cn

[R03] 只读变量
来源：http://lj.jctech888.com.cn

readonly PI=3.14
来源：http://uu.szsharing.cn

[R04] 位置参数
来源：http://qw.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rk.jctech888.com.cn

[R05] 参数默认值
来源：http://jy.9csxet.cn

name="${1:-default}"
来源：http://ya.panjiajie.cn

[R06] 判断命令是否存在
来源：http://zj.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wc.shtwfgs.cn

[R07] if 判断文件
来源：http://cb.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dy.bookmarksfly.cn

[R08] 数值比较
来源：http://zc.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lf.huixiangedu.cn

[R09] 字符串比较
来源：http://oc.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://np.muxihuayi.cn

[R10] 正则匹配
来源：http://mr.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gt.9csxet.cn

[R11] case 多分支
来源：http://er.newstarts.cn


<!-- 参考信息 -->