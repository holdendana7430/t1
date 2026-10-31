代发 wailian999

C#:   Parallel.For
来源：http://ef.szsharing.cn

================================================================================
来源：http://uc.wgjwhj.cn

P. 常用工具函数
来源：http://io.wgjwhj.cn

================================================================================
来源：http://te.wgjwhj.cn

[P01] 生成 UUID
来源：http://xh.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://qj.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tq.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://zu.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://cf.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://ii.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://iy.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://ak.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://no.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://jt.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://un.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ld.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rw.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bp.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nt.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ou.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ho.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dk.lnxyls.cn

[P03] 生成短随机字符串
来源：http://ub.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ey.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dy.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mj.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fz.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iu.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xm.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vg.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gp.huanxung.cn

[P04] 求长度
来源：http://ps.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gu.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ar.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tn.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oq.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://xv.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://ly.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://xj.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qi.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://jp.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bf.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kz.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gp.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://di.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qr.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oj.jianghongdianzi.cn

Ruby: a == b
来源：http://oa.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vi.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://di.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fg.asd995.cn

PHP:  if (empty($x)) {}
来源：http://ri.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ap.shxzukj.cn

TS:   if (x == null) {}
来源：http://gm.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fu.jctech888.com.cn

Go:   if x == nil {}
来源：http://xg.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dz.shxzskj.cn

C#:   if (x is null) {}
来源：http://oj.shtwfgs.cn

[P07] 防抖与节流
来源：http://rg.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uj.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://fg.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lf.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nw.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zx.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rz.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yn.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://ah.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ei.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ju.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nu.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jn.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rn.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oz.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hc.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gh.szsharing.cn

================================================================================
来源：http://hy.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ii.szxytkj.cn

================================================================================
来源：http://wz.wgjwhj.cn

[Q01] 创建表
来源：http://er.hnjuh.cn

CREATE TABLE users (
来源：http://cg.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fu.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://jy.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://ej.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mw.huixinmuqiang.cn

);
来源：http://rn.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://nm.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://pw.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://te.gzmigu.cn

user_id INT NOT NULL,
来源：http://fg.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://cx.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fr.9csxet.cn

);
来源：http://jf.asd995.cn

[Q03] 增加列
来源：http://ib.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hj.huanxung.cn

[Q04] 修改列类型
来源：http://bk.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qe.yuexingan06.cn

[Q05] 重命名列
来源：http://ao.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ud.huanxung.cn

[Q06] 删除列
来源：http://zy.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yl.jianghongdianzi.cn

[Q07] 删除表
来源：http://sw.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://cy.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://tr.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uy.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://gk.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nk.newstarts.cn

[Q10] 插入单行
来源：http://iw.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bo.521024.cn

[Q11] 一次插入多行
来源：http://hr.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jw.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://nu.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ts.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ta.colortex.cn

[Q13] 忽略重复插入
来源：http://ep.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hu.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://wj.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ez.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qp.shtwfgs.cn

[Q15] 查询全部
来源：http://yk.yuexingan06.cn

SELECT * FROM users;
来源：http://ue.muxihuayi.cn

[Q16] 查询指定列
来源：http://se.szsharing.cn

SELECT id, name FROM users;
来源：http://dv.521024.cn

[Q17] 条件查询
来源：http://av.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nx.521024.cn

[Q18] 模糊匹配
来源：http://lh.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cz.hahajie.cn

[Q19] 范围查询
来源：http://tw.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dn.shxzukj.cn

[Q20] IN 列表
来源：http://cz.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qu.hahajie.cn

[Q21] 空值判断
来源：http://zn.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://am.szxytkj.cn

[Q22] 排序
来源：http://es.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tq.huixinmuqiang.cn

[Q23] 分页
来源：http://vb.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xx.asd995.cn

[Q24] 去重
来源：http://te.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://hr.nicolike.cn

[Q25] 只取前 N 条
来源：http://wz.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gu.chemitech.net.cn

[Q26] 计数
来源：http://ff.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://ch.newstarts.cn

[Q27] 条件计数
来源：http://xa.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pa.muxihuayi.cn

[Q28] 求和与平均
来源：http://eq.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tf.szsharing.cn

[Q29] 最大最小值
来源：http://ji.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jt.shxzukj.cn

[Q30] 分组统计
来源：http://hy.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xw.jctech888.com.cn

[Q31] 分组后过滤
来源：http://uy.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vy.huanxung.cn

[Q32] 分组拼接字符串
来源：http://xz.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nf.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gz.bjjhwx.cn

[Q33] 多列分组
来源：http://hy.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zo.jctech888.com.cn

[Q34] 每组取第一条
来源：http://vz.yuntaijiaju.cn

SELECT * FROM (
来源：http://am.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ts.521024.cn

) t WHERE rn = 1;
来源：http://zg.shxzskj.cn

[Q35] 内连接
来源：http://qv.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fv.szsharing.cn

[Q36] 左连接
来源：http://jl.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gg.chemitech.net.cn

[Q37] 右连接
来源：http://km.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://na.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wq.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ck.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://tu.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ex.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nz.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kn.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eq.newstarts.cn

[Q41] 多表连接
来源：http://cx.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://we.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://fe.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://zf.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://db.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://vq.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://na.shtwfgs.cn

[Q43] 标量子查询
来源：http://gz.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yt.chemitech.net.cn

[Q44] IN 子查询
来源：http://ry.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uy.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://hk.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mf.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vx.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://im.nicolike.cn

[Q47] 与平均值比较
来源：http://cn.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kp.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://op.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jf.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://ay.wgjwhj.cn

[Q49] 更新单行
来源：http://rc.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ln.szsharing.cn

[Q50] 批量更新
来源：http://bs.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://de.shxzskj.cn

[Q51] 用子查询更新
来源：http://bt.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ef.gzmigu.cn

[Q52] 删除指定行
来源：http://pu.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://kv.huanxung.cn

[Q53] 按条件删除
来源：http://xo.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mn.huixiangedu.cn

[Q54] 清空表
来源：http://jy.nszjky.cn

TRUNCATE TABLE logs;
来源：http://zs.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://nf.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://od.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://jb.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rd.huanxung.cn

[Q57] 行号
来源：http://yl.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oe.bjjhwx.cn

[Q58] 累计求和
来源：http://ad.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ph.huixiangedu.cn

[Q59] 分组内累计
来源：http://uz.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pb.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://gg.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kc.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://au.muxihuayi.cn

[Q61] 移动平均
来源：http://ie.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://id.bookmarksfly.cn

[Q62] 分组占比
来源：http://go.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qu.shxzskj.cn

[Q63] 开启事务
来源：http://vn.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://re.chemitech.net.cn

[Q64] 提交事务
来源：http://dy.nicolike.cn

COMMIT;
来源：http://sd.bookmarksfly.cn

[Q65] 回滚事务
来源：http://dn.szsharing.cn

ROLLBACK;
来源：http://ts.newstarts.cn

[Q66] 行锁查询
来源：http://cg.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dd.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://pq.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iy.bjjhwx.cn

[Q68] 保存点
来源：http://qm.szsharing.cn

SAVEPOINT sp1;
来源：http://vi.newstarts.cn

ROLLBACK TO sp1;
来源：http://nv.shxzskj.cn

[Q69] 查看执行计划
来源：http://ib.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uf.asd995.cn

[Q70] 更新统计信息
来源：http://ie.haigaiapp.cn

ANALYZE TABLE users;
来源：http://vd.szsharing.cn

[Q71] 查看建表语句
来源：http://rm.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rq.szsharing.cn

[Q72] 查看索引
来源：http://vw.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://pk.panjiajie.cn

[Q73] 查看表状态
来源：http://lj.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pu.shtwfgs.cn

[Q74] 强制使用索引
来源：http://kr.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vf.bookmarksfly.cn

[Q75] 日期格式化
来源：http://io.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dz.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hr.gzmigu.cn

[Q76] 按天统计
来源：http://nu.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nu.hahajie.cn

[Q77] 时间加减
来源：http://vw.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nh.hnjuh.cn

[Q78] 当前时间
来源：http://la.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ew.huixiangedu.cn

[Q79] 字符串拼接
来源：http://cq.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hl.wgjwhj.cn

[Q80] 字符串截取
来源：http://zy.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gl.huanxung.cn

[Q81] 字符串替换
来源：http://fw.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ex.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://hs.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ez.shxzskj.cn

[Q83] 大小写转换
来源：http://lo.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rd.nszjky.cn

[Q84] 去除首尾空格
来源：http://uj.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://fk.newstarts.cn

[Q85] 数值取整
来源：http://uz.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wq.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://oe.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xx.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ol.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jd.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://pl.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nz.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nu.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://hl.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lr.shtwfgs.cn

[Q90] 生成序号列
来源：http://of.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hk.yuntaijiaju.cn

================================================================================
来源：http://la.521024.cn

R. Bash 专题
来源：http://mh.huanxung.cn

================================================================================
来源：http://qh.asd995.cn

[R01] shebang 与严格模式
来源：http://ob.9csxet.cn

#!/usr/bin/env bash
来源：http://mh.huixinmuqiang.cn

set -euo pipefail
来源：http://xr.hahajie.cn

[R02] 变量赋值与使用
来源：http://ju.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://yw.huixiangedu.cn

[R03] 只读变量
来源：http://dq.haigaiapp.cn

readonly PI=3.14
来源：http://yo.jianghongdianzi.cn

[R04] 位置参数
来源：http://qc.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ac.jianghongdianzi.cn

[R05] 参数默认值
来源：http://kh.521024.cn

name="${1:-default}"
来源：http://um.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://hv.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eo.bookmarksfly.cn

[R07] if 判断文件
来源：http://an.jctech888.com.cn


<!-- 参考信息 -->