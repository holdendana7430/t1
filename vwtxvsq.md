代发 wailian999

[P01] 生成 UUID
来源：http://bg.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://oa.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://db.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://dg.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://rj.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://we.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://tm.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://yr.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://ii.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ce.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://er.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mv.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oz.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lz.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uo.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hg.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ry.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dp.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://qm.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cz.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lj.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qb.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rx.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rl.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zo.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rp.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ju.asd995.cn

[P04] 求长度
来源：http://tn.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tw.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://os.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uw.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cn.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://bt.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://uz.shxzskj.cn

Ruby: x.length;  x.size
来源：http://uh.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://an.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://bf.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vy.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://va.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fx.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pv.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sy.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vd.gzmigu.cn

Ruby: a == b
来源：http://ty.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gm.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fz.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gv.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://gs.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gy.bjjhwx.cn

TS:   if (x == null) {}
来源：http://jj.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cl.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://bi.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cw.jctech888.com.cn

C#:   if (x is null) {}
来源：http://br.shxzskj.cn

[P07] 防抖与节流
来源：http://jx.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fi.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://ij.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gn.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zw.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://su.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mf.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gp.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oj.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://fu.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vg.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ru.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ik.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kq.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://id.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ga.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ms.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wu.jctech888.com.cn

================================================================================
来源：http://pz.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://us.asd995.cn

================================================================================
来源：http://gr.hahajie.cn

[Q01] 创建表
来源：http://jc.muxihuayi.cn

CREATE TABLE users (
来源：http://pq.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tk.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://js.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://vq.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sq.szxytkj.cn

);
来源：http://zs.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://hm.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://hn.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ll.szsharing.cn

user_id INT NOT NULL,
来源：http://nd.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://ns.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gc.521024.cn

);
来源：http://wq.huixinmuqiang.cn

[Q03] 增加列
来源：http://pm.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bk.wgjwhj.cn

[Q04] 修改列类型
来源：http://cr.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mr.9csxet.cn

[Q05] 重命名列
来源：http://lh.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qp.haigaiapp.cn

[Q06] 删除列
来源：http://tp.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://me.wgjwhj.cn

[Q07] 删除表
来源：http://rf.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://ft.shxzskj.cn

[Q08] 创建普通索引
来源：http://jd.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rg.shxzskj.cn

[Q09] 创建唯一索引
来源：http://qm.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ei.newstarts.cn

[Q10] 插入单行
来源：http://wv.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bl.lnxyls.cn

[Q11] 一次插入多行
来源：http://af.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gk.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://ef.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://et.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kw.lnxyls.cn

[Q13] 忽略重复插入
来源：http://fd.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rf.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://pr.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zs.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tv.nicolike.cn

[Q15] 查询全部
来源：http://db.szxytkj.cn

SELECT * FROM users;
来源：http://md.yuexingan06.cn

[Q16] 查询指定列
来源：http://ny.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://hu.chemitech.net.cn

[Q17] 条件查询
来源：http://sj.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ft.shxzukj.cn

[Q18] 模糊匹配
来源：http://zy.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pp.szsharing.cn

[Q19] 范围查询
来源：http://xj.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://io.nicolike.cn

[Q20] IN 列表
来源：http://ig.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pu.huanxung.cn

[Q21] 空值判断
来源：http://be.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gx.haigaiapp.cn

[Q22] 排序
来源：http://wd.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iq.gzmigu.cn

[Q23] 分页
来源：http://qe.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qh.wgjwhj.cn

[Q24] 去重
来源：http://mt.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://oj.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://io.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rt.shxzskj.cn

[Q26] 计数
来源：http://wr.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://nk.yuexingan06.cn

[Q27] 条件计数
来源：http://zx.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://je.bjjhwx.cn

[Q28] 求和与平均
来源：http://zu.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ui.hnjuh.cn

[Q29] 最大最小值
来源：http://qj.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hn.asd995.cn

[Q30] 分组统计
来源：http://se.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://on.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://cz.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ck.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://bj.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xy.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kc.shxzukj.cn

[Q33] 多列分组
来源：http://yj.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pz.nicolike.cn

[Q34] 每组取第一条
来源：http://gc.panjiajie.cn

SELECT * FROM (
来源：http://qa.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uy.gzmigu.cn

) t WHERE rn = 1;
来源：http://aw.asd995.cn

[Q35] 内连接
来源：http://bi.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bb.9csxet.cn

[Q36] 左连接
来源：http://rs.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vw.chemitech.net.cn

[Q37] 右连接
来源：http://bt.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qw.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qg.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://er.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ti.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ps.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nh.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ky.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pq.huanxung.cn

[Q41] 多表连接
来源：http://gf.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wv.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ln.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://ep.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://ze.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://aw.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kr.nicolike.cn

[Q43] 标量子查询
来源：http://ic.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wj.nszjky.cn

[Q44] IN 子查询
来源：http://ru.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bz.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://wa.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ln.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ui.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oa.muxihuayi.cn

[Q47] 与平均值比较
来源：http://bx.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://un.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://fl.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hq.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://yk.newstarts.cn

[Q49] 更新单行
来源：http://ph.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tb.shxzskj.cn

[Q50] 批量更新
来源：http://vk.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ub.huixiangedu.cn

[Q51] 用子查询更新
来源：http://ub.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ey.shxzukj.cn

[Q52] 删除指定行
来源：http://ip.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://od.colortex.cn

[Q53] 按条件删除
来源：http://xw.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://za.lnxyls.cn

[Q54] 清空表
来源：http://fl.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://hg.9csxet.cn

[Q55] 排名（并列占位）
来源：http://kh.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hv.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://os.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zr.jctech888.com.cn

[Q57] 行号
来源：http://ro.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qh.521024.cn

[Q58] 累计求和
来源：http://vc.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ww.hahajie.cn

[Q59] 分组内累计
来源：http://ts.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://an.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://pi.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oe.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ji.muxihuayi.cn

[Q61] 移动平均
来源：http://vy.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ih.shxzukj.cn

[Q62] 分组占比
来源：http://fv.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oj.gzmigu.cn

[Q63] 开启事务
来源：http://mm.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oa.colortex.cn

[Q64] 提交事务
来源：http://jx.chemitech.net.cn

COMMIT;
来源：http://hi.newstarts.cn

[Q65] 回滚事务
来源：http://nq.hnjuh.cn

ROLLBACK;
来源：http://vm.wgjwhj.cn

[Q66] 行锁查询
来源：http://gq.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vj.colortex.cn

[Q67] 设置隔离级别
来源：http://us.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ib.nszjky.cn

[Q68] 保存点
来源：http://gu.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://pi.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://dc.jctech888.com.cn

[Q69] 查看执行计划
来源：http://wm.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gu.521024.cn

[Q70] 更新统计信息
来源：http://vt.colortex.cn

ANALYZE TABLE users;
来源：http://ap.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ay.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ik.szsharing.cn

[Q72] 查看索引
来源：http://jf.lnxyls.cn

SHOW INDEX FROM users;
来源：http://qk.yuexingan06.cn

[Q73] 查看表状态
来源：http://rs.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bx.colortex.cn

[Q74] 强制使用索引
来源：http://du.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tg.lnxyls.cn

[Q75] 日期格式化
来源：http://xa.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mx.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zg.wgjwhj.cn

[Q76] 按天统计
来源：http://nw.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uj.nicolike.cn

[Q77] 时间加减
来源：http://hm.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oo.muxihuayi.cn

[Q78] 当前时间
来源：http://pd.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oz.colortex.cn

[Q79] 字符串拼接
来源：http://yq.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pk.colortex.cn

[Q80] 字符串截取
来源：http://nl.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ue.9csxet.cn

[Q81] 字符串替换
来源：http://vh.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ji.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://hg.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dg.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://yb.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iy.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://mq.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://ce.hnjuh.cn

[Q85] 数值取整
来源：http://ti.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gg.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://uh.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wy.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://tq.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://we.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://mg.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vz.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uc.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://ts.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://su.szxytkj.cn

[Q90] 生成序号列
来源：http://tv.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ja.jctech888.com.cn

================================================================================
来源：http://kn.asd995.cn

R. Bash 专题
来源：http://et.panjiajie.cn

================================================================================
来源：http://iw.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://bw.huanxung.cn

#!/usr/bin/env bash
来源：http://yt.nszjky.cn

set -euo pipefail
来源：http://cz.hahajie.cn

[R02] 变量赋值与使用
来源：http://ph.colortex.cn

name="Tom"; echo "$name"
来源：http://cj.shxzskj.cn

[R03] 只读变量
来源：http://mi.shxzukj.cn

readonly PI=3.14
来源：http://uh.chemitech.net.cn

[R04] 位置参数
来源：http://xj.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fr.shxzskj.cn

[R05] 参数默认值
来源：http://ey.521024.cn

name="${1:-default}"
来源：http://jy.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://vg.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ec.nicolike.cn

[R07] if 判断文件
来源：http://xb.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jr.bookmarksfly.cn

[R08] 数值比较
来源：http://ct.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://in.jctech888.com.cn

[R09] 字符串比较
来源：http://tk.hnjuh.cn


<!-- 参考信息 -->