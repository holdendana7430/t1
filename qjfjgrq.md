代发 wailian999

[P01] 生成 UUID
来源：http://zb.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://vr.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://js.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://lh.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://kd.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://sz.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://hz.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://rd.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://pq.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://zc.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xh.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rp.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iv.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wc.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bc.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ii.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mm.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ey.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://at.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uv.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uh.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gp.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://se.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ig.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lp.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ss.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bt.panjiajie.cn

[P04] 求长度
来源：http://ol.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rw.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fm.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fa.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lh.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://yz.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://tq.newstarts.cn

Ruby: x.length;  x.size
来源：http://ik.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bj.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://sh.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bc.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qh.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cg.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qz.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://so.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jy.newstarts.cn

Ruby: a == b
来源：http://jf.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://re.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ye.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bv.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://vz.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yf.9csxet.cn

TS:   if (x == null) {}
来源：http://xg.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dl.chemitech.net.cn

Go:   if x == nil {}
来源：http://la.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vf.jctech888.com.cn

C#:   if (x is null) {}
来源：http://xd.asd995.cn

[P07] 防抖与节流
来源：http://ie.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fb.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://wa.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ko.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://of.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qo.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nl.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aw.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vt.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://qe.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nr.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ay.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jv.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zm.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ln.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ms.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ce.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hi.muxihuayi.cn

================================================================================
来源：http://ue.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://im.521024.cn

================================================================================
来源：http://bb.yuntaijiaju.cn

[Q01] 创建表
来源：http://gz.nszjky.cn

CREATE TABLE users (
来源：http://tp.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ui.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://yg.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ya.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ha.bjjhwx.cn

);
来源：http://hq.9csxet.cn

[Q02] 创建带外键的表
来源：http://ot.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ei.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.shxzskj.cn

user_id INT NOT NULL,
来源：http://at.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://cg.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jj.huixiangedu.cn

);
来源：http://oy.jctech888.com.cn

[Q03] 增加列
来源：http://yb.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gk.szsharing.cn

[Q04] 修改列类型
来源：http://gx.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nb.newstarts.cn

[Q05] 重命名列
来源：http://zs.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ip.hahajie.cn

[Q06] 删除列
来源：http://dw.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://do.newstarts.cn

[Q07] 删除表
来源：http://bl.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://zf.haigaiapp.cn

[Q08] 创建普通索引
来源：http://xq.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vc.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://lq.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mm.nicolike.cn

[Q10] 插入单行
来源：http://xu.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ek.colortex.cn

[Q11] 一次插入多行
来源：http://xy.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gu.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://fi.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hs.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uk.nicolike.cn

[Q13] 忽略重复插入
来源：http://qn.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://br.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://vb.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qx.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://am.wgjwhj.cn

[Q15] 查询全部
来源：http://wg.jianghongdianzi.cn

SELECT * FROM users;
来源：http://yl.newstarts.cn

[Q16] 查询指定列
来源：http://jt.asd995.cn

SELECT id, name FROM users;
来源：http://jt.gzmigu.cn

[Q17] 条件查询
来源：http://gz.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ns.newstarts.cn

[Q18] 模糊匹配
来源：http://wx.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fy.shxzskj.cn

[Q19] 范围查询
来源：http://vi.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ik.newstarts.cn

[Q20] IN 列表
来源：http://lh.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rg.huixiangedu.cn

[Q21] 空值判断
来源：http://ly.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vg.haigaiapp.cn

[Q22] 排序
来源：http://kd.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gw.bjjhwx.cn

[Q23] 分页
来源：http://nt.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zv.yuntaijiaju.cn

[Q24] 去重
来源：http://fu.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://dv.shxzskj.cn

[Q25] 只取前 N 条
来源：http://kj.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://en.jianghongdianzi.cn

[Q26] 计数
来源：http://rb.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://oa.bookmarksfly.cn

[Q27] 条件计数
来源：http://sa.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oe.gzmigu.cn

[Q28] 求和与平均
来源：http://pe.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://db.shtwfgs.cn

[Q29] 最大最小值
来源：http://yl.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bz.huixinmuqiang.cn

[Q30] 分组统计
来源：http://sg.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ks.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://gu.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ai.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://xe.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xv.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rv.shxzukj.cn

[Q33] 多列分组
来源：http://np.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kr.colortex.cn

[Q34] 每组取第一条
来源：http://ez.9csxet.cn

SELECT * FROM (
来源：http://yv.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://no.9csxet.cn

) t WHERE rn = 1;
来源：http://zm.newstarts.cn

[Q35] 内连接
来源：http://fm.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uy.521024.cn

[Q36] 左连接
来源：http://on.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sh.hahajie.cn

[Q37] 右连接
来源：http://ik.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ys.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sz.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xw.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://ke.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pb.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rt.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lg.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ia.newstarts.cn

[Q41] 多表连接
来源：http://jz.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nn.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://gp.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://qf.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://xx.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://rg.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nc.shxzskj.cn

[Q43] 标量子查询
来源：http://rp.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lh.muxihuayi.cn

[Q44] IN 子查询
来源：http://zq.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sp.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://aa.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dw.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ep.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fc.521024.cn

[Q47] 与平均值比较
来源：http://xj.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cd.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://iq.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wj.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hr.jianghongdianzi.cn

[Q49] 更新单行
来源：http://cc.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yt.521024.cn

[Q50] 批量更新
来源：http://tf.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ub.nszjky.cn

[Q51] 用子查询更新
来源：http://tg.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fb.gzmigu.cn

[Q52] 删除指定行
来源：http://xt.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://gt.szxytkj.cn

[Q53] 按条件删除
来源：http://vp.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yx.jctech888.com.cn

[Q54] 清空表
来源：http://sq.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://nh.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://jh.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hx.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ln.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qa.521024.cn

[Q57] 行号
来源：http://dp.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ot.panjiajie.cn

[Q58] 累计求和
来源：http://tl.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vp.huixiangedu.cn

[Q59] 分组内累计
来源：http://fb.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bo.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://jr.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xo.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iz.nszjky.cn

[Q61] 移动平均
来源：http://sy.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hh.yuntaijiaju.cn

[Q62] 分组占比
来源：http://jm.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bj.hnjuh.cn

[Q63] 开启事务
来源：http://cy.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hy.nszjky.cn

[Q64] 提交事务
来源：http://hx.bookmarksfly.cn

COMMIT;
来源：http://nt.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://xy.newstarts.cn

ROLLBACK;
来源：http://fn.bjjhwx.cn

[Q66] 行锁查询
来源：http://xy.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mj.hnjuh.cn

[Q67] 设置隔离级别
来源：http://so.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gy.bookmarksfly.cn

[Q68] 保存点
来源：http://qq.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://ui.nicolike.cn

ROLLBACK TO sp1;
来源：http://lm.hahajie.cn

[Q69] 查看执行计划
来源：http://oz.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hj.bjjhwx.cn

[Q70] 更新统计信息
来源：http://mj.newstarts.cn

ANALYZE TABLE users;
来源：http://pf.shtwfgs.cn

[Q71] 查看建表语句
来源：http://am.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vh.hnjuh.cn

[Q72] 查看索引
来源：http://nv.hahajie.cn

SHOW INDEX FROM users;
来源：http://su.chemitech.net.cn

[Q73] 查看表状态
来源：http://ap.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kd.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://hr.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ij.521024.cn

[Q75] 日期格式化
来源：http://xf.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jo.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fi.nszjky.cn

[Q76] 按天统计
来源：http://qr.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ht.szsharing.cn

[Q77] 时间加减
来源：http://xa.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lo.colortex.cn

[Q78] 当前时间
来源：http://cp.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xq.panjiajie.cn

[Q79] 字符串拼接
来源：http://vb.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://df.nszjky.cn

[Q80] 字符串截取
来源：http://er.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ja.shtwfgs.cn

[Q81] 字符串替换
来源：http://tu.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sh.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://ka.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jh.muxihuayi.cn

[Q83] 大小写转换
来源：http://ek.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ju.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://fc.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://bo.bookmarksfly.cn

[Q85] 数值取整
来源：http://qd.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ob.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://ms.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jz.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ms.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sk.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://is.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://al.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pp.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://cs.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jm.hnjuh.cn

[Q90] 生成序号列
来源：http://vj.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://so.szsharing.cn

================================================================================
来源：http://sg.9csxet.cn

R. Bash 专题
来源：http://aq.hnjuh.cn

================================================================================
来源：http://lg.hahajie.cn

[R01] shebang 与严格模式
来源：http://gv.hnjuh.cn

#!/usr/bin/env bash
来源：http://nj.huixiangedu.cn

set -euo pipefail
来源：http://vr.shxzukj.cn

[R02] 变量赋值与使用
来源：http://jq.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://kw.shxzskj.cn

[R03] 只读变量
来源：http://xv.jianghongdianzi.cn

readonly PI=3.14
来源：http://wa.lnxyls.cn

[R04] 位置参数
来源：http://fl.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qo.asd995.cn

[R05] 参数默认值
来源：http://tz.huanxung.cn

name="${1:-default}"
来源：http://ba.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://me.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xj.521024.cn

[R07] if 判断文件
来源：http://ks.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ww.yuntaijiaju.cn

[R08] 数值比较
来源：http://it.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dg.jianghongdianzi.cn

[R09] 字符串比较
来源：http://rl.bjjhwx.cn


<!-- 参考信息 -->