代发 wailian999

TS:   // child_process / cluster 模块
来源：http://qx.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tk.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wd.hahajie.cn

Ruby: // fork 块
来源：http://yi.szsharing.cn

C#:   Parallel.For
来源：http://mf.newstarts.cn

================================================================================
来源：http://qu.huixinmuqiang.cn

P. 常用工具函数
来源：http://ko.nszjky.cn

================================================================================
来源：http://lb.nicolike.cn

[P01] 生成 UUID
来源：http://hm.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://tf.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ds.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://ww.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://bg.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://ug.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://ao.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://wg.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://lo.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://fs.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ku.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://di.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jd.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pt.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vj.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nk.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gh.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cg.lnxyls.cn

[P03] 生成短随机字符串
来源：http://sx.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nl.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pu.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ob.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kk.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fw.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jn.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zz.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pe.yuexingan06.cn

[P04] 求长度
来源：http://tl.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lz.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ls.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sk.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xa.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://gv.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://mm.gzmigu.cn

Ruby: x.length;  x.size
来源：http://mj.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ga.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://xw.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bk.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tf.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dn.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xz.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://de.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zi.gzmigu.cn

Ruby: a == b
来源：http://kv.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ef.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://my.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xf.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://lr.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ss.panjiajie.cn

TS:   if (x == null) {}
来源：http://ko.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mc.szxytkj.cn

Go:   if x == nil {}
来源：http://rh.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fo.yuexingan06.cn

C#:   if (x is null) {}
来源：http://pg.lnxyls.cn

[P07] 防抖与节流
来源：http://yd.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xc.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://by.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ha.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ce.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uk.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yg.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vx.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://he.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://qn.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gp.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gd.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jr.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yv.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yw.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uk.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mo.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yw.hnjuh.cn

================================================================================
来源：http://fx.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iq.nicolike.cn

================================================================================
来源：http://lo.chemitech.net.cn

[Q01] 创建表
来源：http://sm.yuexingan06.cn

CREATE TABLE users (
来源：http://dy.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ma.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://dn.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://si.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fx.huixinmuqiang.cn

);
来源：http://df.panjiajie.cn

[Q02] 创建带外键的表
来源：http://cd.shtwfgs.cn

CREATE TABLE orders (
来源：http://rv.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ey.lnxyls.cn

user_id INT NOT NULL,
来源：http://tb.nszjky.cn

amount DECIMAL(10, 2),
来源：http://gd.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sn.bookmarksfly.cn

);
来源：http://gm.muxihuayi.cn

[Q03] 增加列
来源：http://uz.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cz.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://on.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fe.asd995.cn

[Q05] 重命名列
来源：http://er.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xr.521024.cn

[Q06] 删除列
来源：http://mx.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kq.521024.cn

[Q07] 删除表
来源：http://ds.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://zl.colortex.cn

[Q08] 创建普通索引
来源：http://oo.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ws.9csxet.cn

[Q09] 创建唯一索引
来源：http://ca.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bf.hahajie.cn

[Q10] 插入单行
来源：http://iz.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dy.hnjuh.cn

[Q11] 一次插入多行
来源：http://cd.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://be.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://tp.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ev.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oh.nicolike.cn

[Q13] 忽略重复插入
来源：http://vl.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lz.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://tg.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uc.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fn.colortex.cn

[Q15] 查询全部
来源：http://pv.jctech888.com.cn

SELECT * FROM users;
来源：http://jv.asd995.cn

[Q16] 查询指定列
来源：http://ea.szxytkj.cn

SELECT id, name FROM users;
来源：http://wl.hahajie.cn

[Q17] 条件查询
来源：http://ut.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oo.chemitech.net.cn

[Q18] 模糊匹配
来源：http://hj.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zp.chemitech.net.cn

[Q19] 范围查询
来源：http://nk.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vm.hahajie.cn

[Q20] IN 列表
来源：http://pc.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://za.wgjwhj.cn

[Q21] 空值判断
来源：http://pv.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cp.newstarts.cn

[Q22] 排序
来源：http://ad.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sn.lnxyls.cn

[Q23] 分页
来源：http://pe.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://at.nicolike.cn

[Q24] 去重
来源：http://tq.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://bc.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://tw.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wy.asd995.cn

[Q26] 计数
来源：http://fg.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://jq.wgjwhj.cn

[Q27] 条件计数
来源：http://rx.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://of.9csxet.cn

[Q28] 求和与平均
来源：http://mn.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://na.shtwfgs.cn

[Q29] 最大最小值
来源：http://xl.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tp.yuntaijiaju.cn

[Q30] 分组统计
来源：http://ud.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ed.shxzskj.cn

[Q31] 分组后过滤
来源：http://af.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nf.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://ux.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hv.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ba.shxzukj.cn

[Q33] 多列分组
来源：http://dk.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rn.muxihuayi.cn

[Q34] 每组取第一条
来源：http://hu.hnjuh.cn

SELECT * FROM (
来源：http://wu.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vi.haigaiapp.cn

) t WHERE rn = 1;
来源：http://ko.hnjuh.cn

[Q35] 内连接
来源：http://wa.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hx.szsharing.cn

[Q36] 左连接
来源：http://ed.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kr.huixinmuqiang.cn

[Q37] 右连接
来源：http://fw.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fh.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://te.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pz.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ta.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ap.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lp.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nj.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ms.colortex.cn

[Q41] 多表连接
来源：http://gh.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rf.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://ao.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://yv.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://nj.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ft.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qt.panjiajie.cn

[Q43] 标量子查询
来源：http://gu.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://md.jctech888.com.cn

[Q44] IN 子查询
来源：http://kn.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://or.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://ig.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dh.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pu.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jg.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ww.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cn.521024.cn

[Q48] CTE 公用表表达式
来源：http://qo.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kd.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://km.521024.cn

[Q49] 更新单行
来源：http://wg.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ho.521024.cn

[Q50] 批量更新
来源：http://mn.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gb.shxzukj.cn

[Q51] 用子查询更新
来源：http://vl.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dw.muxihuayi.cn

[Q52] 删除指定行
来源：http://oj.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://mp.shtwfgs.cn

[Q53] 按条件删除
来源：http://kx.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fr.colortex.cn

[Q54] 清空表
来源：http://dm.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://be.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://mv.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ok.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://tv.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nw.jctech888.com.cn

[Q57] 行号
来源：http://wx.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cj.yuexingan06.cn

[Q58] 累计求和
来源：http://cf.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ff.nicolike.cn

[Q59] 分组内累计
来源：http://qw.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pl.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://de.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pz.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ao.szxytkj.cn

[Q61] 移动平均
来源：http://vo.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yd.haigaiapp.cn

[Q62] 分组占比
来源：http://hp.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iq.nszjky.cn

[Q63] 开启事务
来源：http://ux.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oy.szxytkj.cn

[Q64] 提交事务
来源：http://ur.huixinmuqiang.cn

COMMIT;
来源：http://ps.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://fr.colortex.cn

ROLLBACK;
来源：http://xa.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://gh.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mp.newstarts.cn

[Q67] 设置隔离级别
来源：http://qr.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sz.jctech888.com.cn

[Q68] 保存点
来源：http://oo.huixiangedu.cn

SAVEPOINT sp1;
来源：http://qx.colortex.cn

ROLLBACK TO sp1;
来源：http://qb.bjjhwx.cn

[Q69] 查看执行计划
来源：http://mu.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wk.lnxyls.cn

[Q70] 更新统计信息
来源：http://ia.colortex.cn

ANALYZE TABLE users;
来源：http://es.huanxung.cn

[Q71] 查看建表语句
来源：http://dn.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hr.szxytkj.cn

[Q72] 查看索引
来源：http://pg.nicolike.cn

SHOW INDEX FROM users;
来源：http://yv.haigaiapp.cn

[Q73] 查看表状态
来源：http://cr.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sr.huixiangedu.cn

[Q74] 强制使用索引
来源：http://os.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xr.colortex.cn

[Q75] 日期格式化
来源：http://oq.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bd.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zk.huixinmuqiang.cn

[Q76] 按天统计
来源：http://kq.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jo.panjiajie.cn

[Q77] 时间加减
来源：http://hv.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://az.gzmigu.cn

[Q78] 当前时间
来源：http://on.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sg.wgjwhj.cn

[Q79] 字符串拼接
来源：http://ii.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vd.yuexingan06.cn

[Q80] 字符串截取
来源：http://xe.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yd.asd995.cn

[Q81] 字符串替换
来源：http://dn.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zm.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://yr.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pj.newstarts.cn

[Q83] 大小写转换
来源：http://vo.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gz.9csxet.cn

[Q84] 去除首尾空格
来源：http://vo.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://eo.chemitech.net.cn

[Q85] 数值取整
来源：http://sn.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://du.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://hs.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xc.huanxung.cn

[Q87] JSON 字段做条件
来源：http://wx.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qo.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://hp.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jo.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nv.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://pf.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qr.bjjhwx.cn

[Q90] 生成序号列
来源：http://dz.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gu.wgjwhj.cn

================================================================================
来源：http://jz.newstarts.cn

R. Bash 专题
来源：http://iu.panjiajie.cn

================================================================================
来源：http://nv.9csxet.cn

[R01] shebang 与严格模式
来源：http://li.shxzukj.cn

#!/usr/bin/env bash
来源：http://ax.nszjky.cn

set -euo pipefail
来源：http://fu.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://rh.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://iw.huixiangedu.cn

[R03] 只读变量
来源：http://su.asd995.cn

readonly PI=3.14
来源：http://dh.muxihuayi.cn

[R04] 位置参数
来源：http://uj.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.huixinmuqiang.cn

[R05] 参数默认值
来源：http://ei.lnxyls.cn


<!-- 参考信息 -->