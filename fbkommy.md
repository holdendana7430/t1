代发 wailian999

C#:   Parallel.For
来源：http://xo.szxytkj.cn

================================================================================
来源：http://wj.shxzukj.cn

P. 常用工具函数
来源：http://ps.nicolike.cn

================================================================================
来源：http://zi.shxzskj.cn

[P01] 生成 UUID
来源：http://xc.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://by.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ji.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://wu.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://wy.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://ln.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://hl.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://qe.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://td.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://em.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ny.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xw.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vr.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qt.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fe.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gu.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kh.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://js.asd995.cn

[P03] 生成短随机字符串
来源：http://xr.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ce.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xn.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ub.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rw.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ze.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hd.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oh.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tc.jctech888.com.cn

[P04] 求长度
来源：http://ko.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yl.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xk.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qp.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ml.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://nf.colortex.cn

Go:   len(arr);  len(m)
来源：http://bc.gzmigu.cn

Ruby: x.length;  x.size
来源：http://tj.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://si.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://wy.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qq.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nd.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jy.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fa.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hg.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vi.nicolike.cn

Ruby: a == b
来源：http://md.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qf.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ed.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ek.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://qq.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://li.shxzukj.cn

TS:   if (x == null) {}
来源：http://mm.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fa.bookmarksfly.cn

Go:   if x == nil {}
来源：http://iq.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xf.shxzskj.cn

C#:   if (x is null) {}
来源：http://kn.yuexingan06.cn

[P07] 防抖与节流
来源：http://ij.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dv.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://zc.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sg.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xd.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vh.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://do.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yo.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cz.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://sr.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nm.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ji.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oh.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fe.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jy.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ip.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yf.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uq.shtwfgs.cn

================================================================================
来源：http://ix.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zk.asd995.cn

================================================================================
来源：http://ft.bjjhwx.cn

[Q01] 创建表
来源：http://iw.yuntaijiaju.cn

CREATE TABLE users (
来源：http://qa.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://se.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ug.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://jt.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dx.asd995.cn

);
来源：http://tj.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://fy.jctech888.com.cn

CREATE TABLE orders (
来源：http://an.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dr.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://im.521024.cn

amount DECIMAL(10, 2),
来源：http://fz.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zp.shxzskj.cn

);
来源：http://kv.szxytkj.cn

[Q03] 增加列
来源：http://sf.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://so.colortex.cn

[Q04] 修改列类型
来源：http://jt.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://og.9csxet.cn

[Q05] 重命名列
来源：http://sf.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://py.szxytkj.cn

[Q06] 删除列
来源：http://hl.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rs.yuntaijiaju.cn

[Q07] 删除表
来源：http://or.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://kb.bjjhwx.cn

[Q08] 创建普通索引
来源：http://pa.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hk.9csxet.cn

[Q09] 创建唯一索引
来源：http://rr.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eg.huanxung.cn

[Q10] 插入单行
来源：http://bv.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rx.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ly.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cv.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://mh.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ef.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xp.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://fe.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sr.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://xc.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vp.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qk.nicolike.cn

[Q15] 查询全部
来源：http://fb.lnxyls.cn

SELECT * FROM users;
来源：http://xl.nszjky.cn

[Q16] 查询指定列
来源：http://yv.huixiangedu.cn

SELECT id, name FROM users;
来源：http://pl.chemitech.net.cn

[Q17] 条件查询
来源：http://hx.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uv.huanxung.cn

[Q18] 模糊匹配
来源：http://zb.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wd.shxzukj.cn

[Q19] 范围查询
来源：http://ks.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pl.jctech888.com.cn

[Q20] IN 列表
来源：http://ny.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dr.jctech888.com.cn

[Q21] 空值判断
来源：http://lq.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ke.bookmarksfly.cn

[Q22] 排序
来源：http://zo.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nz.chemitech.net.cn

[Q23] 分页
来源：http://xq.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ni.bjjhwx.cn

[Q24] 去重
来源：http://hp.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://ro.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://ja.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://am.shxzskj.cn

[Q26] 计数
来源：http://gx.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://wn.shtwfgs.cn

[Q27] 条件计数
来源：http://dy.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dq.lnxyls.cn

[Q28] 求和与平均
来源：http://pc.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lj.shxzskj.cn

[Q29] 最大最小值
来源：http://bc.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hv.nicolike.cn

[Q30] 分组统计
来源：http://cx.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gt.nszjky.cn

[Q31] 分组后过滤
来源：http://gs.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hf.szsharing.cn

[Q32] 分组拼接字符串
来源：http://ue.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nq.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ny.nicolike.cn

[Q33] 多列分组
来源：http://nk.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dr.9csxet.cn

[Q34] 每组取第一条
来源：http://kr.szsharing.cn

SELECT * FROM (
来源：http://fr.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lc.yuexingan06.cn

) t WHERE rn = 1;
来源：http://hp.newstarts.cn

[Q35] 内连接
来源：http://ik.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://am.shxzskj.cn

[Q36] 左连接
来源：http://sf.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gq.shtwfgs.cn

[Q37] 右连接
来源：http://ka.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pe.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://df.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ws.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://yd.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gz.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gz.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wu.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qh.colortex.cn

[Q41] 多表连接
来源：http://aj.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://th.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://km.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://uh.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://od.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ev.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yc.wgjwhj.cn

[Q43] 标量子查询
来源：http://se.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kg.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://eb.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ce.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://fz.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ex.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gn.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zq.hahajie.cn

[Q47] 与平均值比较
来源：http://gj.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hy.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://kb.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yh.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://fl.huanxung.cn

[Q49] 更新单行
来源：http://xw.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xa.huixinmuqiang.cn

[Q50] 批量更新
来源：http://mr.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cw.muxihuayi.cn

[Q51] 用子查询更新
来源：http://xc.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rp.521024.cn

[Q52] 删除指定行
来源：http://wm.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://ww.521024.cn

[Q53] 按条件删除
来源：http://if.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://og.hnjuh.cn

[Q54] 清空表
来源：http://du.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://tx.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://sp.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vh.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://ic.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ng.chemitech.net.cn

[Q57] 行号
来源：http://hx.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ff.shxzukj.cn

[Q58] 累计求和
来源：http://te.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wk.hahajie.cn

[Q59] 分组内累计
来源：http://ra.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ii.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://oh.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ni.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rj.colortex.cn

[Q61] 移动平均
来源：http://wv.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qx.9csxet.cn

[Q62] 分组占比
来源：http://sf.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uj.lnxyls.cn

[Q63] 开启事务
来源：http://gc.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sh.wgjwhj.cn

[Q64] 提交事务
来源：http://ym.gzmigu.cn

COMMIT;
来源：http://mm.shxzskj.cn

[Q65] 回滚事务
来源：http://vd.newstarts.cn

ROLLBACK;
来源：http://gt.chemitech.net.cn

[Q66] 行锁查询
来源：http://iy.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ku.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://jy.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ro.shtwfgs.cn

[Q68] 保存点
来源：http://oe.bjjhwx.cn

SAVEPOINT sp1;
来源：http://rd.shxzskj.cn

ROLLBACK TO sp1;
来源：http://xz.9csxet.cn

[Q69] 查看执行计划
来源：http://ph.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ki.chemitech.net.cn

[Q70] 更新统计信息
来源：http://qg.nicolike.cn

ANALYZE TABLE users;
来源：http://ko.asd995.cn

[Q71] 查看建表语句
来源：http://on.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yq.newstarts.cn

[Q72] 查看索引
来源：http://gl.szsharing.cn

SHOW INDEX FROM users;
来源：http://gk.9csxet.cn

[Q73] 查看表状态
来源：http://uf.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ug.yuexingan06.cn

[Q74] 强制使用索引
来源：http://ib.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fe.shxzukj.cn

[Q75] 日期格式化
来源：http://lo.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wq.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ov.hahajie.cn

[Q76] 按天统计
来源：http://ze.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jm.nszjky.cn

[Q77] 时间加减
来源：http://xi.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kk.jianghongdianzi.cn

[Q78] 当前时间
来源：http://xp.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ua.jctech888.com.cn

[Q79] 字符串拼接
来源：http://zn.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ya.szsharing.cn

[Q80] 字符串截取
来源：http://ct.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ug.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://ah.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cj.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://if.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yc.bjjhwx.cn

[Q83] 大小写转换
来源：http://cf.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://po.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://ob.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://ll.gzmigu.cn

[Q85] 数值取整
来源：http://uq.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ru.colortex.cn

[Q86] 读取 JSON 字段
来源：http://go.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zd.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://ca.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yv.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://fe.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gv.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kf.panjiajie.cn

[Q89] 判断表是否存在
来源：http://ko.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ga.hnjuh.cn

[Q90] 生成序号列
来源：http://pw.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cm.wgjwhj.cn

================================================================================
来源：http://hy.yuntaijiaju.cn

R. Bash 专题
来源：http://do.hahajie.cn

================================================================================
来源：http://es.gzmigu.cn

[R01] shebang 与严格模式
来源：http://dv.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://qa.gzmigu.cn

set -euo pipefail
来源：http://ca.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://wz.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://kq.wgjwhj.cn

[R03] 只读变量
来源：http://fu.muxihuayi.cn

readonly PI=3.14
来源：http://ak.yuexingan06.cn

[R04] 位置参数
来源：http://eh.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://li.szsharing.cn

[R05] 参数默认值
来源：http://ke.nszjky.cn

name="${1:-default}"
来源：http://wi.huanxung.cn

[R06] 判断命令是否存在
来源：http://wz.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ij.hnjuh.cn

[R07] if 判断文件
来源：http://fb.haigaiapp.cn


<!-- 参考信息 -->