代发 wailian999

TS:   crypto.randomUUID()
来源：http://lg.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://wv.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://ha.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://ix.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://hf.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://uz.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hu.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jl.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yn.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yr.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dh.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fj.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tz.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kf.shxzukj.cn

[P03] 生成短随机字符串
来源：http://iv.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zs.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://go.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vo.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fv.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pz.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yj.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pk.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zb.gzmigu.cn

[P04] 求长度
来源：http://vt.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cm.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oq.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ah.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ho.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://yi.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://to.panjiajie.cn

Ruby: x.length;  x.size
来源：http://vk.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mt.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://gc.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gx.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xf.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uh.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yq.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cg.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xr.yuntaijiaju.cn

Ruby: a == b
来源：http://ue.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://df.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ka.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jd.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://zf.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lm.jctech888.com.cn

TS:   if (x == null) {}
来源：http://dp.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ee.szsharing.cn

Go:   if x == nil {}
来源：http://ef.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ok.asd995.cn

C#:   if (x is null) {}
来源：http://gr.yuexingan06.cn

[P07] 防抖与节流
来源：http://oi.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://za.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://pb.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://us.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fr.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zs.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lp.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fi.szsharing.cn

[P08] 处理浮点精度问题
来源：http://ew.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uo.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kj.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dz.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ch.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://no.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://en.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wf.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lf.huixinmuqiang.cn

================================================================================
来源：http://ex.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://he.shxzukj.cn

================================================================================
来源：http://qp.lnxyls.cn

[Q01] 创建表
来源：http://vf.jianghongdianzi.cn

CREATE TABLE users (
来源：http://bo.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wr.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://tf.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://yx.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yz.gzmigu.cn

);
来源：http://cy.nszjky.cn

[Q02] 创建带外键的表
来源：http://ir.nicolike.cn

CREATE TABLE orders (
来源：http://ha.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jc.shtwfgs.cn

user_id INT NOT NULL,
来源：http://tp.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://fx.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ji.huixinmuqiang.cn

);
来源：http://fw.wgjwhj.cn

[Q03] 增加列
来源：http://pg.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fd.521024.cn

[Q04] 修改列类型
来源：http://lw.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hv.szxytkj.cn

[Q05] 重命名列
来源：http://hq.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sx.huanxung.cn

[Q06] 删除列
来源：http://pv.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yw.chemitech.net.cn

[Q07] 删除表
来源：http://jo.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ai.shxzskj.cn

[Q08] 创建普通索引
来源：http://jx.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bp.szxytkj.cn

[Q09] 创建唯一索引
来源：http://pl.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iv.bjjhwx.cn

[Q10] 插入单行
来源：http://cl.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fw.szsharing.cn

[Q11] 一次插入多行
来源：http://tf.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://se.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://uc.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ek.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wb.szsharing.cn

[Q13] 忽略重复插入
来源：http://vl.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://il.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://xb.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jb.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bj.wgjwhj.cn

[Q15] 查询全部
来源：http://sx.huixiangedu.cn

SELECT * FROM users;
来源：http://hf.haigaiapp.cn

[Q16] 查询指定列
来源：http://zu.shxzukj.cn

SELECT id, name FROM users;
来源：http://mr.haigaiapp.cn

[Q17] 条件查询
来源：http://hn.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ii.yuexingan06.cn

[Q18] 模糊匹配
来源：http://ib.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://id.huixinmuqiang.cn

[Q19] 范围查询
来源：http://id.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ym.yuexingan06.cn

[Q20] IN 列表
来源：http://cn.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rb.asd995.cn

[Q21] 空值判断
来源：http://jz.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bb.shtwfgs.cn

[Q22] 排序
来源：http://kq.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yf.muxihuayi.cn

[Q23] 分页
来源：http://tb.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yn.bjjhwx.cn

[Q24] 去重
来源：http://qk.521024.cn

SELECT DISTINCT city FROM users;
来源：http://xb.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://es.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ij.nicolike.cn

[Q26] 计数
来源：http://mz.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://wx.szxytkj.cn

[Q27] 条件计数
来源：http://kr.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nl.shxzukj.cn

[Q28] 求和与平均
来源：http://kx.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oj.gzmigu.cn

[Q29] 最大最小值
来源：http://la.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pi.huixinmuqiang.cn

[Q30] 分组统计
来源：http://dg.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wu.szsharing.cn

[Q31] 分组后过滤
来源：http://bx.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ok.hahajie.cn

[Q32] 分组拼接字符串
来源：http://tz.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vj.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ba.jianghongdianzi.cn

[Q33] 多列分组
来源：http://cn.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pr.muxihuayi.cn

[Q34] 每组取第一条
来源：http://vl.jianghongdianzi.cn

SELECT * FROM (
来源：http://zx.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ib.huixiangedu.cn

) t WHERE rn = 1;
来源：http://zd.bjjhwx.cn

[Q35] 内连接
来源：http://rv.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hj.chemitech.net.cn

[Q36] 左连接
来源：http://er.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yv.yuntaijiaju.cn

[Q37] 右连接
来源：http://mn.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gm.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sl.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://om.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://yf.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://if.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dg.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pp.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ce.muxihuayi.cn

[Q41] 多表连接
来源：http://yk.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://og.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://it.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://vs.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://lz.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://dv.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://an.yuexingan06.cn

[Q43] 标量子查询
来源：http://ya.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ne.panjiajie.cn

[Q44] IN 子查询
来源：http://kh.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iw.colortex.cn

[Q45] EXISTS 判断存在
来源：http://or.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dw.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jq.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oo.hnjuh.cn

[Q47] 与平均值比较
来源：http://jz.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ew.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://kn.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ro.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://hz.haigaiapp.cn

[Q49] 更新单行
来源：http://hl.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rs.jctech888.com.cn

[Q50] 批量更新
来源：http://ur.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bj.newstarts.cn

[Q51] 用子查询更新
来源：http://on.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ei.521024.cn

[Q52] 删除指定行
来源：http://wp.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://dr.hahajie.cn

[Q53] 按条件删除
来源：http://zm.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://po.huanxung.cn

[Q54] 清空表
来源：http://sr.huanxung.cn

TRUNCATE TABLE logs;
来源：http://fj.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://jr.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pu.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://jr.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sp.newstarts.cn

[Q57] 行号
来源：http://sq.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hr.yuntaijiaju.cn

[Q58] 累计求和
来源：http://cd.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://do.haigaiapp.cn

[Q59] 分组内累计
来源：http://im.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://na.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://gi.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cz.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://je.hahajie.cn

[Q61] 移动平均
来源：http://rm.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ym.huixinmuqiang.cn

[Q62] 分组占比
来源：http://hi.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vh.nicolike.cn

[Q63] 开启事务
来源：http://li.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vv.colortex.cn

[Q64] 提交事务
来源：http://qe.szsharing.cn

COMMIT;
来源：http://gr.shxzskj.cn

[Q65] 回滚事务
来源：http://oo.asd995.cn

ROLLBACK;
来源：http://zj.hahajie.cn

[Q66] 行锁查询
来源：http://xx.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ap.szxytkj.cn

[Q67] 设置隔离级别
来源：http://nq.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jc.huixinmuqiang.cn

[Q68] 保存点
来源：http://lx.huixiangedu.cn

SAVEPOINT sp1;
来源：http://bp.9csxet.cn

ROLLBACK TO sp1;
来源：http://qb.newstarts.cn

[Q69] 查看执行计划
来源：http://aq.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xu.nicolike.cn

[Q70] 更新统计信息
来源：http://rz.chemitech.net.cn

ANALYZE TABLE users;
来源：http://le.panjiajie.cn

[Q71] 查看建表语句
来源：http://nz.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oe.shxzukj.cn

[Q72] 查看索引
来源：http://in.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://kx.newstarts.cn

[Q73] 查看表状态
来源：http://bn.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aj.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://dt.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rh.szxytkj.cn

[Q75] 日期格式化
来源：http://tq.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://og.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lo.wgjwhj.cn

[Q76] 按天统计
来源：http://ln.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tq.9csxet.cn

[Q77] 时间加减
来源：http://yo.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://se.shxzukj.cn

[Q78] 当前时间
来源：http://rj.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hw.hnjuh.cn

[Q79] 字符串拼接
来源：http://qx.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bw.nszjky.cn

[Q80] 字符串截取
来源：http://zb.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ia.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://uz.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xf.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://nh.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dc.muxihuayi.cn

[Q83] 大小写转换
来源：http://pl.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ow.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://bs.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://qn.huanxung.cn

[Q85] 数值取整
来源：http://gp.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://re.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://ql.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cd.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://fp.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nj.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://yr.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bf.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yq.gzmigu.cn

[Q89] 判断表是否存在
来源：http://lk.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xg.lnxyls.cn

[Q90] 生成序号列
来源：http://fr.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gp.bjjhwx.cn

================================================================================
来源：http://zz.hahajie.cn

R. Bash 专题
来源：http://bo.9csxet.cn

================================================================================
来源：http://rv.nicolike.cn

[R01] shebang 与严格模式
来源：http://sw.newstarts.cn

#!/usr/bin/env bash
来源：http://ed.chemitech.net.cn

set -euo pipefail
来源：http://rz.shxzskj.cn

[R02] 变量赋值与使用
来源：http://du.asd995.cn

name="Tom"; echo "$name"
来源：http://es.szxytkj.cn

[R03] 只读变量
来源：http://ht.jctech888.com.cn

readonly PI=3.14
来源：http://ie.nszjky.cn

[R04] 位置参数
来源：http://ja.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ig.szxytkj.cn

[R05] 参数默认值
来源：http://gp.nicolike.cn

name="${1:-default}"
来源：http://cv.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://lz.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lh.colortex.cn

[R07] if 判断文件
来源：http://gg.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cp.521024.cn

[R08] 数值比较
来源：http://ev.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mp.szsharing.cn

[R09] 字符串比较
来源：http://pt.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://za.hahajie.cn

[R10] 正则匹配
来源：http://tj.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ko.bookmarksfly.cn

[R11] case 多分支
来源：http://wh.jianghongdianzi.cn


<!-- 参考信息 -->