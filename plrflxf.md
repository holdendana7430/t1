代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://cj.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://ce.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kq.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sq.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wf.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dl.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://to.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tx.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jr.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tz.nicolike.cn

[P03] 生成短随机字符串
来源：http://bs.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ha.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ia.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oc.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://na.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wf.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dr.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://he.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bh.wgjwhj.cn

[P04] 求长度
来源：http://nb.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ae.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oy.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rt.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uj.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://pk.newstarts.cn

Go:   len(arr);  len(m)
来源：http://qr.9csxet.cn

Ruby: x.length;  x.size
来源：http://hd.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ae.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://wn.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ow.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uo.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ry.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vu.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bl.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jt.huixinmuqiang.cn

Ruby: a == b
来源：http://jx.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vo.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://el.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ta.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://by.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wj.szxytkj.cn

TS:   if (x == null) {}
来源：http://oo.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ht.haigaiapp.cn

Go:   if x == nil {}
来源：http://ug.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wh.nszjky.cn

C#:   if (x is null) {}
来源：http://xp.colortex.cn

[P07] 防抖与节流
来源：http://jg.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tv.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://vu.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://po.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xl.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tk.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zy.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mx.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rt.szsharing.cn

[P08] 处理浮点精度问题
来源：http://ms.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rk.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yf.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bm.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://io.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ew.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fg.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://px.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://md.jctech888.com.cn

================================================================================
来源：http://wq.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ly.huanxung.cn

================================================================================
来源：http://ye.colortex.cn

[Q01] 创建表
来源：http://hx.yuntaijiaju.cn

CREATE TABLE users (
来源：http://dk.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yc.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://il.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://dw.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sv.shxzskj.cn

);
来源：http://lx.huanxung.cn

[Q02] 创建带外键的表
来源：http://zx.nszjky.cn

CREATE TABLE orders (
来源：http://yw.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ih.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://tz.szsharing.cn

amount DECIMAL(10, 2),
来源：http://vw.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gk.muxihuayi.cn

);
来源：http://jv.colortex.cn

[Q03] 增加列
来源：http://um.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lv.hnjuh.cn

[Q04] 修改列类型
来源：http://ng.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fs.yuexingan06.cn

[Q05] 重命名列
来源：http://rv.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kq.huanxung.cn

[Q06] 删除列
来源：http://dm.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dl.huixinmuqiang.cn

[Q07] 删除表
来源：http://ou.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://fe.panjiajie.cn

[Q08] 创建普通索引
来源：http://jr.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ej.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://mb.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jp.bookmarksfly.cn

[Q10] 插入单行
来源：http://gi.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pv.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://vh.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hw.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://xl.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hq.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ii.521024.cn

[Q13] 忽略重复插入
来源：http://hi.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uy.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://op.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zl.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rv.shtwfgs.cn

[Q15] 查询全部
来源：http://io.yuntaijiaju.cn

SELECT * FROM users;
来源：http://qg.colortex.cn

[Q16] 查询指定列
来源：http://ax.asd995.cn

SELECT id, name FROM users;
来源：http://ww.gzmigu.cn

[Q17] 条件查询
来源：http://ok.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hi.szsharing.cn

[Q18] 模糊匹配
来源：http://gy.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hs.panjiajie.cn

[Q19] 范围查询
来源：http://ij.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ay.muxihuayi.cn

[Q20] IN 列表
来源：http://kk.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dr.szxytkj.cn

[Q21] 空值判断
来源：http://ke.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rk.gzmigu.cn

[Q22] 排序
来源：http://pq.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kz.nicolike.cn

[Q23] 分页
来源：http://tm.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ol.hnjuh.cn

[Q24] 去重
来源：http://ts.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://xf.nszjky.cn

[Q25] 只取前 N 条
来源：http://yf.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pz.huixinmuqiang.cn

[Q26] 计数
来源：http://tl.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://sl.jctech888.com.cn

[Q27] 条件计数
来源：http://kv.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pl.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://cp.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ps.shtwfgs.cn

[Q29] 最大最小值
来源：http://hl.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ph.shxzukj.cn

[Q30] 分组统计
来源：http://sx.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bp.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://jf.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qo.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://wf.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://si.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oo.muxihuayi.cn

[Q33] 多列分组
来源：http://br.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lb.panjiajie.cn

[Q34] 每组取第一条
来源：http://sh.gzmigu.cn

SELECT * FROM (
来源：http://cv.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ws.shtwfgs.cn

) t WHERE rn = 1;
来源：http://ph.chemitech.net.cn

[Q35] 内连接
来源：http://gc.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sb.muxihuayi.cn

[Q36] 左连接
来源：http://ws.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kn.shtwfgs.cn

[Q37] 右连接
来源：http://pz.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bh.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xj.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xt.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://uf.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zm.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xi.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mw.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hm.szxytkj.cn

[Q41] 多表连接
来源：http://cj.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dm.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://wf.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://th.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://on.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://vr.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vz.shtwfgs.cn

[Q43] 标量子查询
来源：http://rw.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rh.muxihuayi.cn

[Q44] IN 子查询
来源：http://kl.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kw.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://vt.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vf.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ui.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rj.szxytkj.cn

[Q47] 与平均值比较
来源：http://mg.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kn.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://zk.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://di.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://gj.panjiajie.cn

[Q49] 更新单行
来源：http://mx.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rh.521024.cn

[Q50] 批量更新
来源：http://ie.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sz.gzmigu.cn

[Q51] 用子查询更新
来源：http://uy.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iy.yuexingan06.cn

[Q52] 删除指定行
来源：http://wn.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://xr.gzmigu.cn

[Q53] 按条件删除
来源：http://yk.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rj.9csxet.cn

[Q54] 清空表
来源：http://sg.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://dl.huanxung.cn

[Q55] 排名（并列占位）
来源：http://fy.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gn.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://up.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sy.nszjky.cn

[Q57] 行号
来源：http://vv.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lf.nicolike.cn

[Q58] 累计求和
来源：http://vj.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tt.wgjwhj.cn

[Q59] 分组内累计
来源：http://tu.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xh.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://ew.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dc.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rq.shxzukj.cn

[Q61] 移动平均
来源：http://vi.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iv.panjiajie.cn

[Q62] 分组占比
来源：http://fl.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pm.jctech888.com.cn

[Q63] 开启事务
来源：http://hd.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ui.haigaiapp.cn

[Q64] 提交事务
来源：http://cm.yuntaijiaju.cn

COMMIT;
来源：http://jj.hnjuh.cn

[Q65] 回滚事务
来源：http://un.bookmarksfly.cn

ROLLBACK;
来源：http://wj.shtwfgs.cn

[Q66] 行锁查询
来源：http://ji.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xg.colortex.cn

[Q67] 设置隔离级别
来源：http://eb.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kp.haigaiapp.cn

[Q68] 保存点
来源：http://is.hnjuh.cn

SAVEPOINT sp1;
来源：http://fi.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://qq.panjiajie.cn

[Q69] 查看执行计划
来源：http://fs.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ag.hnjuh.cn

[Q70] 更新统计信息
来源：http://tp.haigaiapp.cn

ANALYZE TABLE users;
来源：http://kv.hnjuh.cn

[Q71] 查看建表语句
来源：http://yq.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jr.yuntaijiaju.cn

[Q72] 查看索引
来源：http://cq.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://ja.huanxung.cn

[Q73] 查看表状态
来源：http://il.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bw.yuexingan06.cn

[Q74] 强制使用索引
来源：http://uf.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jl.chemitech.net.cn

[Q75] 日期格式化
来源：http://or.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ps.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pl.nszjky.cn

[Q76] 按天统计
来源：http://ri.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://id.gzmigu.cn

[Q77] 时间加减
来源：http://bw.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lp.yuntaijiaju.cn

[Q78] 当前时间
来源：http://yc.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rm.bjjhwx.cn

[Q79] 字符串拼接
来源：http://cg.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yo.shxzskj.cn

[Q80] 字符串截取
来源：http://wx.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dg.shxzukj.cn

[Q81] 字符串替换
来源：http://cj.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wq.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://yj.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sw.newstarts.cn

[Q83] 大小写转换
来源：http://at.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yg.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://pw.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ib.newstarts.cn

[Q85] 数值取整
来源：http://zv.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nj.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://jr.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ph.colortex.cn

[Q87] JSON 字段做条件
来源：http://pu.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://km.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://vi.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fn.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hw.newstarts.cn

[Q89] 判断表是否存在
来源：http://nz.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sa.hnjuh.cn

[Q90] 生成序号列
来源：http://br.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kh.shxzukj.cn

================================================================================
来源：http://qs.chemitech.net.cn

R. Bash 专题
来源：http://hk.jianghongdianzi.cn

================================================================================
来源：http://rd.nszjky.cn

[R01] shebang 与严格模式
来源：http://dk.huanxung.cn

#!/usr/bin/env bash
来源：http://wl.shxzskj.cn

set -euo pipefail
来源：http://cj.gzmigu.cn

[R02] 变量赋值与使用
来源：http://zg.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://ob.9csxet.cn

[R03] 只读变量
来源：http://uv.shxzskj.cn

readonly PI=3.14
来源：http://ja.521024.cn

[R04] 位置参数
来源：http://yh.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yd.yuntaijiaju.cn

[R05] 参数默认值
来源：http://eu.521024.cn

name="${1:-default}"
来源：http://oh.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://qd.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qo.yuexingan06.cn

[R07] if 判断文件
来源：http://wt.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fg.newstarts.cn

[R08] 数值比较
来源：http://ja.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vc.yuntaijiaju.cn

[R09] 字符串比较
来源：http://vw.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hs.hahajie.cn

[R10] 正则匹配
来源：http://uw.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uh.huixinmuqiang.cn

[R11] case 多分支
来源：http://fb.9csxet.cn

case "$1" in
来源：http://yl.shtwfgs.cn

start) echo "启动" ;;
来源：http://up.lnxyls.cn

stop)  echo "停止" ;;
来源：http://zb.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://aa.jctech888.com.cn


<!-- 参考信息 -->