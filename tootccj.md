代发 wailian999

[P01] 生成 UUID
来源：http://bc.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://eb.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sc.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://tb.newstarts.cn

TS:   crypto.randomUUID()
来源：http://ym.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://ur.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ta.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ou.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://fb.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://ox.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qc.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lv.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sv.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sd.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mt.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mw.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mg.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qz.hnjuh.cn

[P03] 生成短随机字符串
来源：http://yt.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mi.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://de.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tt.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zz.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wj.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wo.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nf.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://af.wgjwhj.cn

[P04] 求长度
来源：http://dm.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wh.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pi.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gq.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lo.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://dh.9csxet.cn

Go:   len(arr);  len(m)
来源：http://ac.hahajie.cn

Ruby: x.length;  x.size
来源：http://en.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ai.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://ep.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yl.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wi.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fn.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://du.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oz.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fg.shtwfgs.cn

Ruby: a == b
来源：http://jt.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pm.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yb.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://af.asd995.cn

PHP:  if (empty($x)) {}
来源：http://xn.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ut.muxihuayi.cn

TS:   if (x == null) {}
来源：http://mw.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ae.panjiajie.cn

Go:   if x == nil {}
来源：http://pz.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pm.szxytkj.cn

C#:   if (x is null) {}
来源：http://ri.colortex.cn

[P07] 防抖与节流
来源：http://jx.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cc.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://dx.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ka.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ti.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fa.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zv.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ek.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oq.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://zx.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uu.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://th.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wg.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://un.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mz.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mi.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sg.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bi.bookmarksfly.cn

================================================================================
来源：http://si.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ex.yuntaijiaju.cn

================================================================================
来源：http://qc.shxzskj.cn

[Q01] 创建表
来源：http://tn.huixinmuqiang.cn

CREATE TABLE users (
来源：http://sj.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pc.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://br.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://vr.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wp.szsharing.cn

);
来源：http://eg.szxytkj.cn

[Q02] 创建带外键的表
来源：http://el.gzmigu.cn

CREATE TABLE orders (
来源：http://qy.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://po.hnjuh.cn

user_id INT NOT NULL,
来源：http://ih.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://jr.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bj.huixiangedu.cn

);
来源：http://ow.huanxung.cn

[Q03] 增加列
来源：http://iq.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fm.9csxet.cn

[Q04] 修改列类型
来源：http://zo.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://so.jianghongdianzi.cn

[Q05] 重命名列
来源：http://qs.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://de.haigaiapp.cn

[Q06] 删除列
来源：http://ak.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xk.nicolike.cn

[Q07] 删除表
来源：http://yy.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://ye.shxzukj.cn

[Q08] 创建普通索引
来源：http://qm.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yk.huanxung.cn

[Q09] 创建唯一索引
来源：http://pf.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kt.gzmigu.cn

[Q10] 插入单行
来源：http://ds.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mh.haigaiapp.cn

[Q11] 一次插入多行
来源：http://yo.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kz.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://is.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rs.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://br.huanxung.cn

[Q13] 忽略重复插入
来源：http://mr.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://az.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://tm.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qj.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://us.chemitech.net.cn

[Q15] 查询全部
来源：http://ys.hnjuh.cn

SELECT * FROM users;
来源：http://ub.bookmarksfly.cn

[Q16] 查询指定列
来源：http://kt.haigaiapp.cn

SELECT id, name FROM users;
来源：http://gs.huixinmuqiang.cn

[Q17] 条件查询
来源：http://wa.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hq.gzmigu.cn

[Q18] 模糊匹配
来源：http://ah.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://re.szsharing.cn

[Q19] 范围查询
来源：http://br.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cr.asd995.cn

[Q20] IN 列表
来源：http://xu.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wg.hnjuh.cn

[Q21] 空值判断
来源：http://gs.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ic.hahajie.cn

[Q22] 排序
来源：http://ps.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://as.gzmigu.cn

[Q23] 分页
来源：http://jz.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ae.chemitech.net.cn

[Q24] 去重
来源：http://tr.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://ot.newstarts.cn

[Q25] 只取前 N 条
来源：http://ur.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ew.yuexingan06.cn

[Q26] 计数
来源：http://ln.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://fy.yuntaijiaju.cn

[Q27] 条件计数
来源：http://mx.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sc.colortex.cn

[Q28] 求和与平均
来源：http://jc.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ns.hahajie.cn

[Q29] 最大最小值
来源：http://pg.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ps.jctech888.com.cn

[Q30] 分组统计
来源：http://rm.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kr.panjiajie.cn

[Q31] 分组后过滤
来源：http://ql.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gn.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://rd.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xa.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zx.shxzukj.cn

[Q33] 多列分组
来源：http://sh.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sd.shtwfgs.cn

[Q34] 每组取第一条
来源：http://qy.shxzskj.cn

SELECT * FROM (
来源：http://rw.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cs.shtwfgs.cn

) t WHERE rn = 1;
来源：http://su.bjjhwx.cn

[Q35] 内连接
来源：http://xi.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ux.hahajie.cn

[Q36] 左连接
来源：http://ff.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jb.nicolike.cn

[Q37] 右连接
来源：http://mi.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xd.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yk.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ft.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://si.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pn.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gg.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yp.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gr.yuexingan06.cn

[Q41] 多表连接
来源：http://ra.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cc.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://mz.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://gk.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://ur.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://sj.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ik.huixiangedu.cn

[Q43] 标量子查询
来源：http://ud.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ye.bjjhwx.cn

[Q44] IN 子查询
来源：http://ds.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vs.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://pq.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sw.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sr.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sp.szsharing.cn

[Q47] 与平均值比较
来源：http://ns.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tt.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://vw.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eg.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://ib.nicolike.cn

[Q49] 更新单行
来源：http://tv.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ze.jianghongdianzi.cn

[Q50] 批量更新
来源：http://wa.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://an.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://ss.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ei.lnxyls.cn

[Q52] 删除指定行
来源：http://tz.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://si.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://so.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ro.szsharing.cn

[Q54] 清空表
来源：http://oz.newstarts.cn

TRUNCATE TABLE logs;
来源：http://aq.9csxet.cn

[Q55] 排名（并列占位）
来源：http://zd.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yj.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://pj.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zi.shxzskj.cn

[Q57] 行号
来源：http://rh.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ui.nicolike.cn

[Q58] 累计求和
来源：http://vi.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://my.bjjhwx.cn

[Q59] 分组内累计
来源：http://pd.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ya.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://pf.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lp.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yx.haigaiapp.cn

[Q61] 移动平均
来源：http://hb.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cj.wgjwhj.cn

[Q62] 分组占比
来源：http://hk.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wq.bjjhwx.cn

[Q63] 开启事务
来源：http://ot.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dp.chemitech.net.cn

[Q64] 提交事务
来源：http://mk.szxytkj.cn

COMMIT;
来源：http://mp.szxytkj.cn

[Q65] 回滚事务
来源：http://jp.asd995.cn

ROLLBACK;
来源：http://nk.bookmarksfly.cn

[Q66] 行锁查询
来源：http://yj.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gb.huanxung.cn

[Q67] 设置隔离级别
来源：http://jk.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ut.huixiangedu.cn

[Q68] 保存点
来源：http://cc.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://wa.gzmigu.cn

ROLLBACK TO sp1;
来源：http://ej.haigaiapp.cn

[Q69] 查看执行计划
来源：http://pa.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hb.muxihuayi.cn

[Q70] 更新统计信息
来源：http://oz.hahajie.cn

ANALYZE TABLE users;
来源：http://hp.huanxung.cn

[Q71] 查看建表语句
来源：http://nx.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rc.lnxyls.cn

[Q72] 查看索引
来源：http://by.9csxet.cn

SHOW INDEX FROM users;
来源：http://pi.muxihuayi.cn

[Q73] 查看表状态
来源：http://fc.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iw.9csxet.cn

[Q74] 强制使用索引
来源：http://gy.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fv.gzmigu.cn

[Q75] 日期格式化
来源：http://pj.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pt.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fn.panjiajie.cn

[Q76] 按天统计
来源：http://ji.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qs.szsharing.cn

[Q77] 时间加减
来源：http://uu.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qo.chemitech.net.cn

[Q78] 当前时间
来源：http://gp.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ai.wgjwhj.cn

[Q79] 字符串拼接
来源：http://gw.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hb.newstarts.cn

[Q80] 字符串截取
来源：http://wp.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://np.szsharing.cn

[Q81] 字符串替换
来源：http://ec.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mw.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://vb.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jp.gzmigu.cn

[Q83] 大小写转换
来源：http://ae.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cc.huanxung.cn

[Q84] 去除首尾空格
来源：http://hp.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://om.huixiangedu.cn

[Q85] 数值取整
来源：http://rm.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yn.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://pk.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ew.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://zd.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://su.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://fx.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hv.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cv.nicolike.cn

[Q89] 判断表是否存在
来源：http://rd.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dn.chemitech.net.cn

[Q90] 生成序号列
来源：http://ek.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://db.szxytkj.cn

================================================================================
来源：http://iv.szsharing.cn

R. Bash 专题
来源：http://me.hnjuh.cn

================================================================================
来源：http://ny.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://ds.521024.cn

#!/usr/bin/env bash
来源：http://dq.bookmarksfly.cn

set -euo pipefail
来源：http://wd.nicolike.cn

[R02] 变量赋值与使用
来源：http://jg.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://oh.haigaiapp.cn

[R03] 只读变量
来源：http://qv.asd995.cn

readonly PI=3.14
来源：http://vg.shtwfgs.cn

[R04] 位置参数
来源：http://uj.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kk.shtwfgs.cn

[R05] 参数默认值
来源：http://oc.haigaiapp.cn

name="${1:-default}"
来源：http://zv.panjiajie.cn

[R06] 判断命令是否存在
来源：http://by.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tu.asd995.cn

[R07] if 判断文件
来源：http://ev.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ug.huanxung.cn

[R08] 数值比较
来源：http://ph.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ym.jianghongdianzi.cn

[R09] 字符串比较
来源：http://jc.nicolike.cn


<!-- 参考信息 -->