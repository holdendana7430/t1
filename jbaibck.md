代发 wailian999

C#:   Parallel.For
来源：http://lh.haigaiapp.cn

================================================================================
来源：http://ht.lnxyls.cn

P. 常用工具函数
来源：http://rh.szxytkj.cn

================================================================================
来源：http://ll.gzmigu.cn

[P01] 生成 UUID
来源：http://kk.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://oh.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hr.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://cp.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://dm.521024.cn

Java: UUID.randomUUID().toString()
来源：http://sc.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://fa.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ky.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://rp.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://ih.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vj.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rv.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ms.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xg.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qb.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zt.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lw.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ts.gzmigu.cn

[P03] 生成短随机字符串
来源：http://nj.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ak.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://he.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dx.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ta.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hb.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hx.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cw.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nq.yuntaijiaju.cn

[P04] 求长度
来源：http://zc.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://an.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sl.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xb.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://el.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://vj.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://yp.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://vv.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sa.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://bx.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iy.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://na.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ox.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://me.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lb.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lg.yuntaijiaju.cn

Ruby: a == b
来源：http://zp.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aq.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nn.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dq.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://cs.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fn.9csxet.cn

TS:   if (x == null) {}
来源：http://as.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cz.asd995.cn

Go:   if x == nil {}
来源：http://xj.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nn.wgjwhj.cn

C#:   if (x is null) {}
来源：http://hm.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://uy.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wa.asd995.cn

PHP:  // 手写时间戳比较
来源：http://fd.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xu.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mq.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hp.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rb.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vd.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://br.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://cd.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vc.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qo.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ja.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cs.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iu.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ny.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ff.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dx.9csxet.cn

================================================================================
来源：http://tv.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wu.huixiangedu.cn

================================================================================
来源：http://uk.yuntaijiaju.cn

[Q01] 创建表
来源：http://ec.panjiajie.cn

CREATE TABLE users (
来源：http://io.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tw.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://ne.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://kd.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oh.hahajie.cn

);
来源：http://hi.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://ay.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://xh.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ly.jctech888.com.cn

user_id INT NOT NULL,
来源：http://wl.colortex.cn

amount DECIMAL(10, 2),
来源：http://kk.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qq.wgjwhj.cn

);
来源：http://gz.huanxung.cn

[Q03] 增加列
来源：http://el.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mc.nicolike.cn

[Q04] 修改列类型
来源：http://zb.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uc.haigaiapp.cn

[Q05] 重命名列
来源：http://cn.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://au.bookmarksfly.cn

[Q06] 删除列
来源：http://iy.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vu.shtwfgs.cn

[Q07] 删除表
来源：http://ej.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://yw.hnjuh.cn

[Q08] 创建普通索引
来源：http://rx.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jj.newstarts.cn

[Q09] 创建唯一索引
来源：http://ew.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cx.gzmigu.cn

[Q10] 插入单行
来源：http://ty.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wt.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://rk.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jl.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://hi.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://be.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qi.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://lc.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ia.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://xt.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ci.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://is.panjiajie.cn

[Q15] 查询全部
来源：http://lx.haigaiapp.cn

SELECT * FROM users;
来源：http://wv.asd995.cn

[Q16] 查询指定列
来源：http://ca.gzmigu.cn

SELECT id, name FROM users;
来源：http://bs.szsharing.cn

[Q17] 条件查询
来源：http://pe.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zm.9csxet.cn

[Q18] 模糊匹配
来源：http://ce.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://by.jctech888.com.cn

[Q19] 范围查询
来源：http://le.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qn.szsharing.cn

[Q20] IN 列表
来源：http://az.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hg.huanxung.cn

[Q21] 空值判断
来源：http://cj.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lt.nszjky.cn

[Q22] 排序
来源：http://fe.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ph.nszjky.cn

[Q23] 分页
来源：http://wi.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tr.jianghongdianzi.cn

[Q24] 去重
来源：http://qk.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://mf.nszjky.cn

[Q25] 只取前 N 条
来源：http://nq.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yb.asd995.cn

[Q26] 计数
来源：http://ie.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://gs.szsharing.cn

[Q27] 条件计数
来源：http://il.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tp.szxytkj.cn

[Q28] 求和与平均
来源：http://io.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yw.shxzukj.cn

[Q29] 最大最小值
来源：http://oj.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qj.bjjhwx.cn

[Q30] 分组统计
来源：http://dd.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vk.lnxyls.cn

[Q31] 分组后过滤
来源：http://ln.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kz.9csxet.cn

[Q32] 分组拼接字符串
来源：http://px.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gx.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vc.shxzukj.cn

[Q33] 多列分组
来源：http://tw.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://no.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ut.hahajie.cn

SELECT * FROM (
来源：http://pa.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sm.shxzukj.cn

) t WHERE rn = 1;
来源：http://tr.shxzukj.cn

[Q35] 内连接
来源：http://vv.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tq.newstarts.cn

[Q36] 左连接
来源：http://kf.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xr.gzmigu.cn

[Q37] 右连接
来源：http://lz.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uo.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pi.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zp.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://ih.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nj.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wt.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jn.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yt.shtwfgs.cn

[Q41] 多表连接
来源：http://rp.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pa.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://qz.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://af.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://jm.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://oc.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wy.chemitech.net.cn

[Q43] 标量子查询
来源：http://gz.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bl.nszjky.cn

[Q44] IN 子查询
来源：http://wd.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nm.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://re.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iw.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://he.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://os.asd995.cn

[Q47] 与平均值比较
来源：http://mw.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rp.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://ss.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yf.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://mf.nszjky.cn

[Q49] 更新单行
来源：http://ep.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ga.shtwfgs.cn

[Q50] 批量更新
来源：http://yb.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uc.hahajie.cn

[Q51] 用子查询更新
来源：http://xa.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pe.gzmigu.cn

[Q52] 删除指定行
来源：http://qn.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://cs.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://dt.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vr.yuexingan06.cn

[Q54] 清空表
来源：http://so.nicolike.cn

TRUNCATE TABLE logs;
来源：http://al.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ke.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tn.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://yr.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fs.newstarts.cn

[Q57] 行号
来源：http://fo.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wm.nicolike.cn

[Q58] 累计求和
来源：http://ya.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rl.panjiajie.cn

[Q59] 分组内累计
来源：http://oi.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ao.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://fl.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ol.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ll.yuexingan06.cn

[Q61] 移动平均
来源：http://hs.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://if.haigaiapp.cn

[Q62] 分组占比
来源：http://ay.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://io.szxytkj.cn

[Q63] 开启事务
来源：http://dt.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xa.lnxyls.cn

[Q64] 提交事务
来源：http://cc.lnxyls.cn

COMMIT;
来源：http://zr.wgjwhj.cn

[Q65] 回滚事务
来源：http://fv.huixinmuqiang.cn

ROLLBACK;
来源：http://np.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://fw.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yk.lnxyls.cn

[Q67] 设置隔离级别
来源：http://wj.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://po.521024.cn

[Q68] 保存点
来源：http://eb.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://hd.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://fa.szxytkj.cn

[Q69] 查看执行计划
来源：http://ph.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jg.szsharing.cn

[Q70] 更新统计信息
来源：http://gd.jctech888.com.cn

ANALYZE TABLE users;
来源：http://ez.jctech888.com.cn

[Q71] 查看建表语句
来源：http://rj.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bj.shxzskj.cn

[Q72] 查看索引
来源：http://qa.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://tr.bookmarksfly.cn

[Q73] 查看表状态
来源：http://oh.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://do.shxzskj.cn

[Q74] 强制使用索引
来源：http://rk.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://de.gzmigu.cn

[Q75] 日期格式化
来源：http://kc.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://px.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yf.huanxung.cn

[Q76] 按天统计
来源：http://lm.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wk.jctech888.com.cn

[Q77] 时间加减
来源：http://po.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eb.yuexingan06.cn

[Q78] 当前时间
来源：http://ow.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uz.jctech888.com.cn

[Q79] 字符串拼接
来源：http://na.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gg.lnxyls.cn

[Q80] 字符串截取
来源：http://lr.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nf.bookmarksfly.cn

[Q81] 字符串替换
来源：http://lz.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cv.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://mq.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fy.huanxung.cn

[Q83] 大小写转换
来源：http://jf.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hp.9csxet.cn

[Q84] 去除首尾空格
来源：http://lp.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://gp.colortex.cn

[Q85] 数值取整
来源：http://wd.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wc.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://gj.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xc.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://jy.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://es.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://zy.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ns.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dq.nszjky.cn

[Q89] 判断表是否存在
来源：http://ww.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kx.muxihuayi.cn

[Q90] 生成序号列
来源：http://oj.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xs.shxzskj.cn

================================================================================
来源：http://gn.gzmigu.cn

R. Bash 专题
来源：http://ux.panjiajie.cn

================================================================================
来源：http://qa.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://ic.asd995.cn

#!/usr/bin/env bash
来源：http://zm.colortex.cn

set -euo pipefail
来源：http://fm.9csxet.cn

[R02] 变量赋值与使用
来源：http://hr.szsharing.cn

name="Tom"; echo "$name"
来源：http://sr.chemitech.net.cn

[R03] 只读变量
来源：http://nz.muxihuayi.cn

readonly PI=3.14
来源：http://gz.jianghongdianzi.cn

[R04] 位置参数
来源：http://pd.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bn.huixiangedu.cn

[R05] 参数默认值
来源：http://yb.wgjwhj.cn

name="${1:-default}"
来源：http://be.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://qx.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kz.haigaiapp.cn

[R07] if 判断文件
来源：http://rh.huixinmuqiang.cn


<!-- 参考信息 -->