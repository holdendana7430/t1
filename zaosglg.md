代发 wailian999

TS:   crypto.randomUUID()
来源：http://su.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://pk.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://no.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://wm.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://dh.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://ae.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cf.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ks.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lx.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lm.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lt.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wq.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ge.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oz.521024.cn

[P03] 生成短随机字符串
来源：http://oj.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ds.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jv.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wa.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wp.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fb.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ix.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://td.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ns.nszjky.cn

[P04] 求长度
来源：http://qz.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ra.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xl.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vl.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fs.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://qb.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://nk.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://wg.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://om.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://ub.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iv.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cz.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tl.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://je.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ev.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ri.szsharing.cn

Ruby: a == b
来源：http://bc.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pq.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oe.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://et.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://zk.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wv.colortex.cn

TS:   if (x == null) {}
来源：http://ir.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nz.shtwfgs.cn

Go:   if x == nil {}
来源：http://nq.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yd.wgjwhj.cn

C#:   if (x is null) {}
来源：http://yz.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://vy.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ln.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://aw.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hk.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yn.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://in.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ye.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fi.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://bl.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://in.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kk.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sa.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wb.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hc.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://de.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qk.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://by.colortex.cn

================================================================================
来源：http://zu.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ku.shxzskj.cn

================================================================================
来源：http://qd.colortex.cn

[Q01] 创建表
来源：http://cd.wgjwhj.cn

CREATE TABLE users (
来源：http://hu.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fv.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://hp.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://bh.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ty.muxihuayi.cn

);
来源：http://fb.panjiajie.cn

[Q02] 创建带外键的表
来源：http://hk.gzmigu.cn

CREATE TABLE orders (
来源：http://rs.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tv.asd995.cn

user_id INT NOT NULL,
来源：http://km.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://ax.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mm.nicolike.cn

);
来源：http://eg.asd995.cn

[Q03] 增加列
来源：http://sn.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ae.asd995.cn

[Q04] 修改列类型
来源：http://li.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mr.haigaiapp.cn

[Q05] 重命名列
来源：http://fy.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gw.chemitech.net.cn

[Q06] 删除列
来源：http://xy.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lx.nicolike.cn

[Q07] 删除表
来源：http://yk.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://pl.yuexingan06.cn

[Q08] 创建普通索引
来源：http://sp.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xl.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://ru.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xd.wgjwhj.cn

[Q10] 插入单行
来源：http://kd.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jy.shxzskj.cn

[Q11] 一次插入多行
来源：http://ql.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lw.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://hp.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://px.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vz.panjiajie.cn

[Q13] 忽略重复插入
来源：http://lz.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xi.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://ax.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oy.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ah.bookmarksfly.cn

[Q15] 查询全部
来源：http://ft.huanxung.cn

SELECT * FROM users;
来源：http://nt.hnjuh.cn

[Q16] 查询指定列
来源：http://vn.szsharing.cn

SELECT id, name FROM users;
来源：http://ss.bjjhwx.cn

[Q17] 条件查询
来源：http://wt.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xy.muxihuayi.cn

[Q18] 模糊匹配
来源：http://qp.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dx.haigaiapp.cn

[Q19] 范围查询
来源：http://yj.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://el.huixinmuqiang.cn

[Q20] IN 列表
来源：http://wu.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mx.yuntaijiaju.cn

[Q21] 空值判断
来源：http://qb.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://to.newstarts.cn

[Q22] 排序
来源：http://mf.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oj.szsharing.cn

[Q23] 分页
来源：http://vx.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ho.shxzskj.cn

[Q24] 去重
来源：http://lu.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://ef.521024.cn

[Q25] 只取前 N 条
来源：http://wn.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cu.newstarts.cn

[Q26] 计数
来源：http://qh.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://hz.jianghongdianzi.cn

[Q27] 条件计数
来源：http://rf.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pf.yuexingan06.cn

[Q28] 求和与平均
来源：http://zy.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ho.chemitech.net.cn

[Q29] 最大最小值
来源：http://lq.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xw.lnxyls.cn

[Q30] 分组统计
来源：http://wm.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://my.shxzskj.cn

[Q31] 分组后过滤
来源：http://vp.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gl.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://zo.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qk.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hl.shtwfgs.cn

[Q33] 多列分组
来源：http://rv.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://za.bjjhwx.cn

[Q34] 每组取第一条
来源：http://ds.jctech888.com.cn

SELECT * FROM (
来源：http://sz.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hf.hahajie.cn

) t WHERE rn = 1;
来源：http://fd.jctech888.com.cn

[Q35] 内连接
来源：http://wy.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fr.lnxyls.cn

[Q36] 左连接
来源：http://am.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ho.jianghongdianzi.cn

[Q37] 右连接
来源：http://mr.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tz.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ln.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rn.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://km.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nd.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ib.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dy.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xp.nicolike.cn

[Q41] 多表连接
来源：http://yi.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ea.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://ab.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://pn.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://lz.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://sa.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dz.huanxung.cn

[Q43] 标量子查询
来源：http://ug.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kx.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://fi.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ln.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://lu.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lv.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fb.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fm.wgjwhj.cn

[Q47] 与平均值比较
来源：http://oj.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tc.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://hv.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qd.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://bc.gzmigu.cn

[Q49] 更新单行
来源：http://ap.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://za.jctech888.com.cn

[Q50] 批量更新
来源：http://pr.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fg.nicolike.cn

[Q51] 用子查询更新
来源：http://ww.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gu.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://tq.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://bb.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://eu.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sm.jianghongdianzi.cn

[Q54] 清空表
来源：http://vx.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://fg.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://ca.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yn.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://sl.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gy.nicolike.cn

[Q57] 行号
来源：http://nn.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hy.newstarts.cn

[Q58] 累计求和
来源：http://pa.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vm.nicolike.cn

[Q59] 分组内累计
来源：http://ww.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pi.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://ov.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tj.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nz.yuexingan06.cn

[Q61] 移动平均
来源：http://gr.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ln.jctech888.com.cn

[Q62] 分组占比
来源：http://la.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vg.asd995.cn

[Q63] 开启事务
来源：http://iq.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://us.hahajie.cn

[Q64] 提交事务
来源：http://nd.jianghongdianzi.cn

COMMIT;
来源：http://yj.wgjwhj.cn

[Q65] 回滚事务
来源：http://ii.asd995.cn

ROLLBACK;
来源：http://rk.jctech888.com.cn

[Q66] 行锁查询
来源：http://is.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://km.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://yq.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.szxytkj.cn

[Q68] 保存点
来源：http://mq.jctech888.com.cn

SAVEPOINT sp1;
来源：http://vb.colortex.cn

ROLLBACK TO sp1;
来源：http://hc.nicolike.cn

[Q69] 查看执行计划
来源：http://ie.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bq.shxzukj.cn

[Q70] 更新统计信息
来源：http://lc.muxihuayi.cn

ANALYZE TABLE users;
来源：http://vp.9csxet.cn

[Q71] 查看建表语句
来源：http://ox.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kw.nicolike.cn

[Q72] 查看索引
来源：http://wj.colortex.cn

SHOW INDEX FROM users;
来源：http://sk.szsharing.cn

[Q73] 查看表状态
来源：http://un.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cn.hahajie.cn

[Q74] 强制使用索引
来源：http://ft.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ij.521024.cn

[Q75] 日期格式化
来源：http://zv.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tf.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jb.lnxyls.cn

[Q76] 按天统计
来源：http://gk.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kh.yuexingan06.cn

[Q77] 时间加减
来源：http://fo.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://de.colortex.cn

[Q78] 当前时间
来源：http://bm.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ld.wgjwhj.cn

[Q79] 字符串拼接
来源：http://ek.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oj.9csxet.cn

[Q80] 字符串截取
来源：http://np.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pm.yuexingan06.cn

[Q81] 字符串替换
来源：http://wp.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xt.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://ny.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gj.nicolike.cn

[Q83] 大小写转换
来源：http://yb.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vk.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://pb.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://pd.jctech888.com.cn

[Q85] 数值取整
来源：http://sg.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tn.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://qt.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bs.colortex.cn

[Q87] JSON 字段做条件
来源：http://nw.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ub.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://uz.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://un.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mj.9csxet.cn

[Q89] 判断表是否存在
来源：http://qj.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hg.newstarts.cn

[Q90] 生成序号列
来源：http://on.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ia.huixinmuqiang.cn

================================================================================
来源：http://pg.newstarts.cn

R. Bash 专题
来源：http://ue.haigaiapp.cn

================================================================================
来源：http://ch.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://bu.huixiangedu.cn

#!/usr/bin/env bash
来源：http://mr.gzmigu.cn

set -euo pipefail
来源：http://wm.newstarts.cn

[R02] 变量赋值与使用
来源：http://cp.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://ik.521024.cn

[R03] 只读变量
来源：http://gw.nicolike.cn

readonly PI=3.14
来源：http://mx.nicolike.cn

[R04] 位置参数
来源：http://go.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cg.shxzskj.cn

[R05] 参数默认值
来源：http://rh.nszjky.cn

name="${1:-default}"
来源：http://re.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://dg.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://no.9csxet.cn

[R07] if 判断文件
来源：http://xf.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tk.huixinmuqiang.cn

[R08] 数值比较
来源：http://mf.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rz.panjiajie.cn

[R09] 字符串比较
来源：http://xa.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nw.lnxyls.cn

[R10] 正则匹配
来源：http://ic.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yj.yuexingan06.cn

[R11] case 多分支
来源：http://bw.chemitech.net.cn


<!-- 参考信息 -->