代发 wailian999

TS:   crypto.randomUUID()
来源：http://gd.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://fw.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://ne.521024.cn

Ruby: SecureRandom.uuid
来源：http://og.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://rv.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://gv.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sl.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pf.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mo.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xd.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fr.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ek.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vk.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ss.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://ie.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fg.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ow.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://er.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kp.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cn.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hd.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jr.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pu.muxihuayi.cn

[P04] 求长度
来源：http://gr.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rp.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ep.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fs.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oa.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://ub.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://zg.huanxung.cn

Ruby: x.length;  x.size
来源：http://nt.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ns.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://cc.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ch.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fo.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lb.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ni.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ju.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kg.szxytkj.cn

Ruby: a == b
来源：http://xo.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pa.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wo.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ck.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://io.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wa.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://te.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fq.lnxyls.cn

Go:   if x == nil {}
来源：http://gn.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wo.huanxung.cn

C#:   if (x is null) {}
来源：http://wn.jctech888.com.cn

[P07] 防抖与节流
来源：http://cd.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dq.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://xj.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cs.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ph.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ah.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rt.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nx.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://me.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://bv.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sq.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wl.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://an.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bw.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mk.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ad.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nt.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hg.wgjwhj.cn

================================================================================
来源：http://xr.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://io.bjjhwx.cn

================================================================================
来源：http://ix.yuexingan06.cn

[Q01] 创建表
来源：http://un.shxzukj.cn

CREATE TABLE users (
来源：http://dr.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ab.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://md.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://sf.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wx.huixinmuqiang.cn

);
来源：http://ep.huanxung.cn

[Q02] 创建带外键的表
来源：http://ev.haigaiapp.cn

CREATE TABLE orders (
来源：http://ma.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tv.huanxung.cn

user_id INT NOT NULL,
来源：http://cd.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://bs.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dj.lnxyls.cn

);
来源：http://dh.jianghongdianzi.cn

[Q03] 增加列
来源：http://tg.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qy.szsharing.cn

[Q04] 修改列类型
来源：http://md.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lw.9csxet.cn

[Q05] 重命名列
来源：http://mp.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kj.szxytkj.cn

[Q06] 删除列
来源：http://bo.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xf.gzmigu.cn

[Q07] 删除表
来源：http://iu.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://ny.shxzukj.cn

[Q08] 创建普通索引
来源：http://qc.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ux.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://bf.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bl.gzmigu.cn

[Q10] 插入单行
来源：http://ud.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://im.huanxung.cn

[Q11] 一次插入多行
来源：http://jo.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wr.521024.cn

[Q12] 插入后取自增 ID
来源：http://ju.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ut.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fl.huanxung.cn

[Q13] 忽略重复插入
来源：http://he.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rz.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ok.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lg.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xc.hahajie.cn

[Q15] 查询全部
来源：http://sn.chemitech.net.cn

SELECT * FROM users;
来源：http://cv.9csxet.cn

[Q16] 查询指定列
来源：http://ub.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://uh.colortex.cn

[Q17] 条件查询
来源：http://ds.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rn.nicolike.cn

[Q18] 模糊匹配
来源：http://ki.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dc.shtwfgs.cn

[Q19] 范围查询
来源：http://hu.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gn.nszjky.cn

[Q20] IN 列表
来源：http://zu.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wj.shxzskj.cn

[Q21] 空值判断
来源：http://if.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pg.szxytkj.cn

[Q22] 排序
来源：http://kt.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ec.shxzskj.cn

[Q23] 分页
来源：http://fv.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cw.yuexingan06.cn

[Q24] 去重
来源：http://tl.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://gw.panjiajie.cn

[Q25] 只取前 N 条
来源：http://sz.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cc.asd995.cn

[Q26] 计数
来源：http://oa.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://yv.szxytkj.cn

[Q27] 条件计数
来源：http://bx.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qu.szsharing.cn

[Q28] 求和与平均
来源：http://jx.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ww.colortex.cn

[Q29] 最大最小值
来源：http://ez.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nw.yuexingan06.cn

[Q30] 分组统计
来源：http://ke.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ir.gzmigu.cn

[Q31] 分组后过滤
来源：http://pr.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lq.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://rj.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ei.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uk.newstarts.cn

[Q33] 多列分组
来源：http://ux.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sg.colortex.cn

[Q34] 每组取第一条
来源：http://hn.jctech888.com.cn

SELECT * FROM (
来源：http://ar.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://np.yuexingan06.cn

) t WHERE rn = 1;
来源：http://vm.huixinmuqiang.cn

[Q35] 内连接
来源：http://ab.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yn.bjjhwx.cn

[Q36] 左连接
来源：http://kh.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vq.colortex.cn

[Q37] 右连接
来源：http://qu.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sb.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tz.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rm.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://tb.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ot.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cz.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ke.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mj.gzmigu.cn

[Q41] 多表连接
来源：http://go.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gx.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://ue.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://ia.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://vh.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ju.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zk.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://ed.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://up.lnxyls.cn

[Q44] IN 子查询
来源：http://on.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xq.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://be.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ys.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ui.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yv.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ej.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oe.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://ot.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://on.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://yc.hahajie.cn

[Q49] 更新单行
来源：http://tp.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tr.hnjuh.cn

[Q50] 批量更新
来源：http://kd.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gg.lnxyls.cn

[Q51] 用子查询更新
来源：http://xv.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yy.lnxyls.cn

[Q52] 删除指定行
来源：http://vm.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://wl.colortex.cn

[Q53] 按条件删除
来源：http://rs.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bq.shxzskj.cn

[Q54] 清空表
来源：http://th.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://pw.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://nh.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gr.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://bs.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hg.muxihuayi.cn

[Q57] 行号
来源：http://pa.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mg.nicolike.cn

[Q58] 累计求和
来源：http://ap.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jb.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://dk.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jj.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://cc.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vk.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://el.gzmigu.cn

[Q61] 移动平均
来源：http://cr.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ka.panjiajie.cn

[Q62] 分组占比
来源：http://ey.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bz.jianghongdianzi.cn

[Q63] 开启事务
来源：http://mi.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vj.yuntaijiaju.cn

[Q64] 提交事务
来源：http://nn.lnxyls.cn

COMMIT;
来源：http://oj.shxzskj.cn

[Q65] 回滚事务
来源：http://dy.yuexingan06.cn

ROLLBACK;
来源：http://qb.jctech888.com.cn

[Q66] 行锁查询
来源：http://nr.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nl.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://is.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sj.hnjuh.cn

[Q68] 保存点
来源：http://cd.9csxet.cn

SAVEPOINT sp1;
来源：http://zx.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://vd.szsharing.cn

[Q69] 查看执行计划
来源：http://cu.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qc.panjiajie.cn

[Q70] 更新统计信息
来源：http://ak.chemitech.net.cn

ANALYZE TABLE users;
来源：http://vm.bjjhwx.cn

[Q71] 查看建表语句
来源：http://at.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sx.muxihuayi.cn

[Q72] 查看索引
来源：http://qp.hnjuh.cn

SHOW INDEX FROM users;
来源：http://gn.szsharing.cn

[Q73] 查看表状态
来源：http://bd.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xa.muxihuayi.cn

[Q74] 强制使用索引
来源：http://qn.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sd.hahajie.cn

[Q75] 日期格式化
来源：http://ka.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://an.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://di.panjiajie.cn

[Q76] 按天统计
来源：http://mw.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cl.yuexingan06.cn

[Q77] 时间加减
来源：http://tl.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hf.panjiajie.cn

[Q78] 当前时间
来源：http://ex.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pz.shxzskj.cn

[Q79] 字符串拼接
来源：http://it.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bv.521024.cn

[Q80] 字符串截取
来源：http://ym.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gc.9csxet.cn

[Q81] 字符串替换
来源：http://hi.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tz.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://vq.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ew.nszjky.cn

[Q83] 大小写转换
来源：http://lh.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xn.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://fk.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://ym.shtwfgs.cn

[Q85] 数值取整
来源：http://bj.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xd.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://ez.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mm.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://vp.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fp.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://sb.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ep.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dd.szxytkj.cn

[Q89] 判断表是否存在
来源：http://rk.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qw.shtwfgs.cn

[Q90] 生成序号列
来源：http://zz.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rl.muxihuayi.cn

================================================================================
来源：http://ke.panjiajie.cn

R. Bash 专题
来源：http://gz.chemitech.net.cn

================================================================================
来源：http://va.9csxet.cn

[R01] shebang 与严格模式
来源：http://nt.jctech888.com.cn

#!/usr/bin/env bash
来源：http://ok.panjiajie.cn

set -euo pipefail
来源：http://bv.colortex.cn

[R02] 变量赋值与使用
来源：http://db.521024.cn

name="Tom"; echo "$name"
来源：http://oi.gzmigu.cn

[R03] 只读变量
来源：http://ud.hnjuh.cn

readonly PI=3.14
来源：http://kz.bookmarksfly.cn

[R04] 位置参数
来源：http://em.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cy.szxytkj.cn

[R05] 参数默认值
来源：http://lb.yuntaijiaju.cn

name="${1:-default}"
来源：http://bt.newstarts.cn

[R06] 判断命令是否存在
来源：http://vl.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ih.huixinmuqiang.cn

[R07] if 判断文件
来源：http://un.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dr.hnjuh.cn

[R08] 数值比较
来源：http://ze.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gd.bookmarksfly.cn

[R09] 字符串比较
来源：http://dh.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sq.521024.cn

[R10] 正则匹配
来源：http://ib.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ab.jctech888.com.cn

[R11] case 多分支
来源：http://ko.huixiangedu.cn


<!-- 参考信息 -->