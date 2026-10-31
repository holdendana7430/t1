代发 wailian999

TS:   // child_process / cluster 模块
来源：http://uc.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vm.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://he.hnjuh.cn

Ruby: // fork 块
来源：http://es.lnxyls.cn

C#:   Parallel.For
来源：http://os.huixinmuqiang.cn

================================================================================
来源：http://wn.huixinmuqiang.cn

P. 常用工具函数
来源：http://ik.newstarts.cn

================================================================================
来源：http://jj.hnjuh.cn

[P01] 生成 UUID
来源：http://iw.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://we.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ch.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://eh.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://xa.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://id.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ar.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://mc.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://xc.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://cc.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oe.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://he.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cd.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xj.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://az.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://th.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jz.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vx.colortex.cn

[P03] 生成短随机字符串
来源：http://oa.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zy.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://om.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xl.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wp.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yi.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://br.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pc.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sk.chemitech.net.cn

[P04] 求长度
来源：http://eg.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sq.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dr.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cw.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gh.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://le.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ej.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://lr.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bk.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://qt.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qq.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jl.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sp.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zx.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qt.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gj.muxihuayi.cn

Ruby: a == b
来源：http://yl.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uy.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mm.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cv.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://ys.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yj.shxzukj.cn

TS:   if (x == null) {}
来源：http://ex.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zc.hnjuh.cn

Go:   if x == nil {}
来源：http://pg.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vm.szxytkj.cn

C#:   if (x is null) {}
来源：http://ik.shtwfgs.cn

[P07] 防抖与节流
来源：http://mq.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://if.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://xi.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zt.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xm.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ak.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ky.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rt.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ec.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://my.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gi.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bf.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bc.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kj.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ml.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bo.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wi.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ae.szxytkj.cn

================================================================================
来源：http://rf.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://on.colortex.cn

================================================================================
来源：http://ya.shtwfgs.cn

[Q01] 创建表
来源：http://ds.bjjhwx.cn

CREATE TABLE users (
来源：http://pg.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xk.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://su.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://vg.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sx.shtwfgs.cn

);
来源：http://eq.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://rv.gzmigu.cn

CREATE TABLE orders (
来源：http://zr.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zq.hahajie.cn

user_id INT NOT NULL,
来源：http://ft.colortex.cn

amount DECIMAL(10, 2),
来源：http://of.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fo.shxzukj.cn

);
来源：http://jk.yuntaijiaju.cn

[Q03] 增加列
来源：http://ct.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nv.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://kp.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mv.wgjwhj.cn

[Q05] 重命名列
来源：http://rm.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qr.colortex.cn

[Q06] 删除列
来源：http://ep.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nt.asd995.cn

[Q07] 删除表
来源：http://zw.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://xw.chemitech.net.cn

[Q08] 创建普通索引
来源：http://xp.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vu.szsharing.cn

[Q09] 创建唯一索引
来源：http://gy.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gc.yuntaijiaju.cn

[Q10] 插入单行
来源：http://wi.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xg.shxzskj.cn

[Q11] 一次插入多行
来源：http://ac.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ek.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://fn.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bz.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yn.gzmigu.cn

[Q13] 忽略重复插入
来源：http://gp.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wn.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://as.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yd.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zy.shtwfgs.cn

[Q15] 查询全部
来源：http://po.huanxung.cn

SELECT * FROM users;
来源：http://yr.huanxung.cn

[Q16] 查询指定列
来源：http://ru.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://se.panjiajie.cn

[Q17] 条件查询
来源：http://pi.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bv.jctech888.com.cn

[Q18] 模糊匹配
来源：http://lk.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jk.yuntaijiaju.cn

[Q19] 范围查询
来源：http://ly.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cg.bjjhwx.cn

[Q20] IN 列表
来源：http://pt.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jq.huixinmuqiang.cn

[Q21] 空值判断
来源：http://lo.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://az.shxzukj.cn

[Q22] 排序
来源：http://bk.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rm.huixiangedu.cn

[Q23] 分页
来源：http://ns.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vp.bookmarksfly.cn

[Q24] 去重
来源：http://on.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://fd.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://oi.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ac.shxzskj.cn

[Q26] 计数
来源：http://ha.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://cu.yuexingan06.cn

[Q27] 条件计数
来源：http://rw.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cw.szsharing.cn

[Q28] 求和与平均
来源：http://yq.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iq.muxihuayi.cn

[Q29] 最大最小值
来源：http://iy.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qc.jianghongdianzi.cn

[Q30] 分组统计
来源：http://ft.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cx.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://br.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aj.colortex.cn

[Q32] 分组拼接字符串
来源：http://vy.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://si.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xt.szxytkj.cn

[Q33] 多列分组
来源：http://yq.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ri.lnxyls.cn

[Q34] 每组取第一条
来源：http://wz.yuntaijiaju.cn

SELECT * FROM (
来源：http://gr.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ji.hnjuh.cn

) t WHERE rn = 1;
来源：http://uk.newstarts.cn

[Q35] 内连接
来源：http://qj.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://um.muxihuayi.cn

[Q36] 左连接
来源：http://ik.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pp.szxytkj.cn

[Q37] 右连接
来源：http://aa.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rh.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qh.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bj.asd995.cn

[Q39] 自连接（查上下级）
来源：http://cw.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://om.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sn.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vr.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yq.nszjky.cn

[Q41] 多表连接
来源：http://yz.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oj.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://mu.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://wq.asd995.cn

[Q42] 连接条件附加过滤
来源：http://lh.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://xz.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wc.jctech888.com.cn

[Q43] 标量子查询
来源：http://ok.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bp.colortex.cn

[Q44] IN 子查询
来源：http://kw.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://br.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://pn.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bm.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fd.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qs.yuexingan06.cn

[Q47] 与平均值比较
来源：http://yf.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nw.asd995.cn

[Q48] CTE 公用表表达式
来源：http://me.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jk.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://pe.huixinmuqiang.cn

[Q49] 更新单行
来源：http://co.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kk.huixiangedu.cn

[Q50] 批量更新
来源：http://wx.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ad.wgjwhj.cn

[Q51] 用子查询更新
来源：http://nf.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ur.huanxung.cn

[Q52] 删除指定行
来源：http://iy.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://yq.shxzskj.cn

[Q53] 按条件删除
来源：http://xo.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ko.521024.cn

[Q54] 清空表
来源：http://ue.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://xb.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://xr.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wa.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://ld.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kp.shxzukj.cn

[Q57] 行号
来源：http://oo.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hf.asd995.cn

[Q58] 累计求和
来源：http://ye.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gy.shtwfgs.cn

[Q59] 分组内累计
来源：http://cs.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fd.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://nk.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bp.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wa.bookmarksfly.cn

[Q61] 移动平均
来源：http://fa.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ey.szxytkj.cn

[Q62] 分组占比
来源：http://nx.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iu.shtwfgs.cn

[Q63] 开启事务
来源：http://fi.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mc.hnjuh.cn

[Q64] 提交事务
来源：http://wm.bjjhwx.cn

COMMIT;
来源：http://id.wgjwhj.cn

[Q65] 回滚事务
来源：http://is.muxihuayi.cn

ROLLBACK;
来源：http://vt.hahajie.cn

[Q66] 行锁查询
来源：http://ka.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tz.lnxyls.cn

[Q67] 设置隔离级别
来源：http://uw.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kz.bookmarksfly.cn

[Q68] 保存点
来源：http://zl.gzmigu.cn

SAVEPOINT sp1;
来源：http://fx.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://os.asd995.cn

[Q69] 查看执行计划
来源：http://zb.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lg.colortex.cn

[Q70] 更新统计信息
来源：http://wa.521024.cn

ANALYZE TABLE users;
来源：http://jh.colortex.cn

[Q71] 查看建表语句
来源：http://of.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kj.bjjhwx.cn

[Q72] 查看索引
来源：http://dy.hahajie.cn

SHOW INDEX FROM users;
来源：http://jw.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://qd.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ys.nszjky.cn

[Q74] 强制使用索引
来源：http://mr.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nw.shtwfgs.cn

[Q75] 日期格式化
来源：http://nv.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qb.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fz.haigaiapp.cn

[Q76] 按天统计
来源：http://ia.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ts.shxzukj.cn

[Q77] 时间加减
来源：http://sf.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cg.haigaiapp.cn

[Q78] 当前时间
来源：http://zv.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xs.haigaiapp.cn

[Q79] 字符串拼接
来源：http://yr.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nx.gzmigu.cn

[Q80] 字符串截取
来源：http://ig.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wg.shxzukj.cn

[Q81] 字符串替换
来源：http://ln.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cm.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://zr.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ff.lnxyls.cn

[Q83] 大小写转换
来源：http://qj.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vy.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://lx.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://zv.shtwfgs.cn

[Q85] 数值取整
来源：http://af.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://po.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://nq.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yn.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://hr.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bz.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://zh.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://im.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ns.szsharing.cn

[Q89] 判断表是否存在
来源：http://xu.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uv.panjiajie.cn

[Q90] 生成序号列
来源：http://xb.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ku.shtwfgs.cn

================================================================================
来源：http://xp.newstarts.cn

R. Bash 专题
来源：http://yj.jctech888.com.cn

================================================================================
来源：http://oa.nicolike.cn

[R01] shebang 与严格模式
来源：http://sz.wgjwhj.cn

#!/usr/bin/env bash
来源：http://re.hnjuh.cn

set -euo pipefail
来源：http://rz.nicolike.cn

[R02] 变量赋值与使用
来源：http://hp.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ul.asd995.cn

[R03] 只读变量
来源：http://qx.9csxet.cn

readonly PI=3.14
来源：http://qp.9csxet.cn

[R04] 位置参数
来源：http://rm.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uu.shxzskj.cn

[R05] 参数默认值
来源：http://gr.szsharing.cn


<!-- 参考信息 -->