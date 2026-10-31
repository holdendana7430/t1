代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iz.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://es.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ed.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://md.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uv.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ne.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://rf.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eo.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hv.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pq.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kz.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nt.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ul.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oj.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iq.9csxet.cn

[P04] 求长度
来源：http://cd.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jh.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rw.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qd.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://da.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://dy.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://fw.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://bz.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://am.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://wx.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dp.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lh.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hv.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ar.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fz.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://av.huixiangedu.cn

Ruby: a == b
来源：http://iu.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dz.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cp.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ra.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://hf.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ab.colortex.cn

TS:   if (x == null) {}
来源：http://ww.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ar.hahajie.cn

Go:   if x == nil {}
来源：http://ax.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ql.wgjwhj.cn

C#:   if (x is null) {}
来源：http://lj.gzmigu.cn

[P07] 防抖与节流
来源：http://wh.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://po.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://es.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ql.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gl.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tt.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pb.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nk.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ux.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://tg.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://np.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xj.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vt.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aj.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qv.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xx.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qe.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jm.lnxyls.cn

================================================================================
来源：http://ml.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aq.asd995.cn

================================================================================
来源：http://oo.gzmigu.cn

[Q01] 创建表
来源：http://ba.521024.cn

CREATE TABLE users (
来源：http://ci.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ir.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://hq.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://lf.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rc.nszjky.cn

);
来源：http://tz.hnjuh.cn

[Q02] 创建带外键的表
来源：http://fh.wgjwhj.cn

CREATE TABLE orders (
来源：http://cy.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xn.shxzskj.cn

user_id INT NOT NULL,
来源：http://ce.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://el.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ae.huixinmuqiang.cn

);
来源：http://cn.jianghongdianzi.cn

[Q03] 增加列
来源：http://yd.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oh.lnxyls.cn

[Q04] 修改列类型
来源：http://dh.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mr.jctech888.com.cn

[Q05] 重命名列
来源：http://uo.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ca.szsharing.cn

[Q06] 删除列
来源：http://ra.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lz.nicolike.cn

[Q07] 删除表
来源：http://nu.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://bj.bjjhwx.cn

[Q08] 创建普通索引
来源：http://pp.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wt.gzmigu.cn

[Q09] 创建唯一索引
来源：http://wf.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fe.bjjhwx.cn

[Q10] 插入单行
来源：http://gk.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ch.nszjky.cn

[Q11] 一次插入多行
来源：http://pv.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nx.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://yp.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ew.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lf.shxzskj.cn

[Q13] 忽略重复插入
来源：http://wu.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bh.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://pf.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fq.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fs.bookmarksfly.cn

[Q15] 查询全部
来源：http://zg.szxytkj.cn

SELECT * FROM users;
来源：http://lr.szsharing.cn

[Q16] 查询指定列
来源：http://zq.shxzukj.cn

SELECT id, name FROM users;
来源：http://qi.haigaiapp.cn

[Q17] 条件查询
来源：http://ks.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://om.lnxyls.cn

[Q18] 模糊匹配
来源：http://rw.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vm.huixinmuqiang.cn

[Q19] 范围查询
来源：http://gh.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ya.bjjhwx.cn

[Q20] IN 列表
来源：http://rc.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qh.hahajie.cn

[Q21] 空值判断
来源：http://nn.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jl.asd995.cn

[Q22] 排序
来源：http://jk.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tv.shtwfgs.cn

[Q23] 分页
来源：http://eg.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eo.hnjuh.cn

[Q24] 去重
来源：http://he.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://ui.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://tq.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bf.gzmigu.cn

[Q26] 计数
来源：http://uj.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://xp.asd995.cn

[Q27] 条件计数
来源：http://fk.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tf.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://zt.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://it.chemitech.net.cn

[Q29] 最大最小值
来源：http://fv.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mc.9csxet.cn

[Q30] 分组统计
来源：http://yb.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nb.9csxet.cn

[Q31] 分组后过滤
来源：http://fo.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rm.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://ad.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kx.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mb.yuexingan06.cn

[Q33] 多列分组
来源：http://nv.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ib.panjiajie.cn

[Q34] 每组取第一条
来源：http://sd.yuexingan06.cn

SELECT * FROM (
来源：http://ru.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ht.521024.cn

) t WHERE rn = 1;
来源：http://ba.huixinmuqiang.cn

[Q35] 内连接
来源：http://ij.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cp.bookmarksfly.cn

[Q36] 左连接
来源：http://ic.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zj.9csxet.cn

[Q37] 右连接
来源：http://gx.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://er.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pb.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ae.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://yp.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bi.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ua.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dk.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rs.huixinmuqiang.cn

[Q41] 多表连接
来源：http://of.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wc.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://px.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://vi.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://pl.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ur.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kv.521024.cn

[Q43] 标量子查询
来源：http://nv.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nl.szsharing.cn

[Q44] IN 子查询
来源：http://fq.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yu.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://qz.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://in.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hw.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kl.bjjhwx.cn

[Q47] 与平均值比较
来源：http://fj.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dw.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://mi.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uf.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ey.shxzukj.cn

[Q49] 更新单行
来源：http://qj.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gr.shtwfgs.cn

[Q50] 批量更新
来源：http://ap.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dn.nicolike.cn

[Q51] 用子查询更新
来源：http://fh.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ga.bookmarksfly.cn

[Q52] 删除指定行
来源：http://qc.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://wd.bookmarksfly.cn

[Q53] 按条件删除
来源：http://uy.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sn.huanxung.cn

[Q54] 清空表
来源：http://sl.colortex.cn

TRUNCATE TABLE logs;
来源：http://jq.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://yl.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pk.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://wv.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qs.shxzskj.cn

[Q57] 行号
来源：http://bt.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ve.lnxyls.cn

[Q58] 累计求和
来源：http://mx.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xw.hahajie.cn

[Q59] 分组内累计
来源：http://gk.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ug.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://hp.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pu.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zy.haigaiapp.cn

[Q61] 移动平均
来源：http://mw.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rq.asd995.cn

[Q62] 分组占比
来源：http://lp.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://le.gzmigu.cn

[Q63] 开启事务
来源：http://kv.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://op.yuexingan06.cn

[Q64] 提交事务
来源：http://cp.nicolike.cn

COMMIT;
来源：http://dr.yuexingan06.cn

[Q65] 回滚事务
来源：http://lf.bookmarksfly.cn

ROLLBACK;
来源：http://mv.lnxyls.cn

[Q66] 行锁查询
来源：http://yv.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wt.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://vp.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wu.chemitech.net.cn

[Q68] 保存点
来源：http://kx.hnjuh.cn

SAVEPOINT sp1;
来源：http://ge.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://cf.chemitech.net.cn

[Q69] 查看执行计划
来源：http://ba.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ms.szxytkj.cn

[Q70] 更新统计信息
来源：http://ab.bjjhwx.cn

ANALYZE TABLE users;
来源：http://hq.gzmigu.cn

[Q71] 查看建表语句
来源：http://wj.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://te.bookmarksfly.cn

[Q72] 查看索引
来源：http://mz.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://xh.lnxyls.cn

[Q73] 查看表状态
来源：http://ht.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ur.shxzukj.cn

[Q74] 强制使用索引
来源：http://xx.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yu.hahajie.cn

[Q75] 日期格式化
来源：http://ck.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gi.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oa.jctech888.com.cn

[Q76] 按天统计
来源：http://zs.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tr.huixiangedu.cn

[Q77] 时间加减
来源：http://kk.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hd.shtwfgs.cn

[Q78] 当前时间
来源：http://dn.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cx.hahajie.cn

[Q79] 字符串拼接
来源：http://in.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qi.521024.cn

[Q80] 字符串截取
来源：http://fd.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ht.gzmigu.cn

[Q81] 字符串替换
来源：http://xj.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xh.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://gk.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://os.bookmarksfly.cn

[Q83] 大小写转换
来源：http://gp.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ub.hnjuh.cn

[Q84] 去除首尾空格
来源：http://ir.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://gp.shxzskj.cn

[Q85] 数值取整
来源：http://ii.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pi.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://ju.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sg.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://hi.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lu.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ao.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://it.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ql.szxytkj.cn

[Q89] 判断表是否存在
来源：http://tc.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yz.521024.cn

[Q90] 生成序号列
来源：http://nb.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rb.nicolike.cn

================================================================================
来源：http://me.muxihuayi.cn

R. Bash 专题
来源：http://yu.szxytkj.cn

================================================================================
来源：http://yf.hnjuh.cn

[R01] shebang 与严格模式
来源：http://dk.szsharing.cn

#!/usr/bin/env bash
来源：http://rm.panjiajie.cn

set -euo pipefail
来源：http://st.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://hn.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://nh.colortex.cn

[R03] 只读变量
来源：http://dj.yuexingan06.cn

readonly PI=3.14
来源：http://kb.wgjwhj.cn

[R04] 位置参数
来源：http://cl.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cq.huanxung.cn

[R05] 参数默认值
来源：http://ul.shtwfgs.cn

name="${1:-default}"
来源：http://pi.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://kc.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ec.shtwfgs.cn

[R07] if 判断文件
来源：http://hg.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ea.bjjhwx.cn

[R08] 数值比较
来源：http://ar.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bf.panjiajie.cn

[R09] 字符串比较
来源：http://kv.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gd.chemitech.net.cn

[R10] 正则匹配
来源：http://ym.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ms.yuexingan06.cn

[R11] case 多分支
来源：http://gi.huixinmuqiang.cn

case "$1" in
来源：http://zt.szxytkj.cn

start) echo "启动" ;;
来源：http://kf.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://mc.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://ty.huixinmuqiang.cn

esac
来源：http://fp.hahajie.cn

[R12] for 遍历文件
来源：http://qx.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://rb.nszjky.cn

[R13] for 计数循环
来源：http://xb.hahajie.cn


<!-- 参考信息 -->