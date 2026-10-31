代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://ly.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://we.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://af.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kb.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zs.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fd.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oj.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tp.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://px.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jm.lnxyls.cn

[P03] 生成短随机字符串
来源：http://co.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nh.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yo.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qi.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jj.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://km.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ad.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nu.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lt.huixiangedu.cn

[P04] 求长度
来源：http://ys.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bc.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://av.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dp.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ha.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://ow.panjiajie.cn

Ruby: x.length;  x.size
来源：http://ga.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ff.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://gl.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fl.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://es.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wf.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mn.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cj.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hv.9csxet.cn

Ruby: a == b
来源：http://ft.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ws.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xe.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ud.colortex.cn

PHP:  if (empty($x)) {}
来源：http://pa.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yk.shtwfgs.cn

TS:   if (x == null) {}
来源：http://sz.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wq.nszjky.cn

Go:   if x == nil {}
来源：http://mf.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fx.szsharing.cn

C#:   if (x is null) {}
来源：http://ik.muxihuayi.cn

[P07] 防抖与节流
来源：http://vm.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bt.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://wv.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ss.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://el.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ff.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://um.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yh.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ff.huanxung.cn

[P08] 处理浮点精度问题
来源：http://hl.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://om.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kr.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ug.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ja.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://os.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lo.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ne.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oa.huanxung.cn

================================================================================
来源：http://oq.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lv.asd995.cn

================================================================================
来源：http://hg.521024.cn

[Q01] 创建表
来源：http://al.asd995.cn

CREATE TABLE users (
来源：http://qw.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tu.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://zq.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://gg.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ge.chemitech.net.cn

);
来源：http://ke.hahajie.cn

[Q02] 创建带外键的表
来源：http://cn.9csxet.cn

CREATE TABLE orders (
来源：http://gt.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dd.szxytkj.cn

user_id INT NOT NULL,
来源：http://vq.521024.cn

amount DECIMAL(10, 2),
来源：http://my.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nv.colortex.cn

);
来源：http://hu.huixiangedu.cn

[Q03] 增加列
来源：http://jk.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yv.huixiangedu.cn

[Q04] 修改列类型
来源：http://os.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hq.huanxung.cn

[Q05] 重命名列
来源：http://iu.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xe.521024.cn

[Q06] 删除列
来源：http://hf.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vi.hahajie.cn

[Q07] 删除表
来源：http://iz.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://la.shtwfgs.cn

[Q08] 创建普通索引
来源：http://tu.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fv.colortex.cn

[Q09] 创建唯一索引
来源：http://wd.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yg.szsharing.cn

[Q10] 插入单行
来源：http://td.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mn.jctech888.com.cn

[Q11] 一次插入多行
来源：http://df.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://us.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://na.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wd.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vl.gzmigu.cn

[Q13] 忽略重复插入
来源：http://dy.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zf.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://je.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yk.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hj.huixinmuqiang.cn

[Q15] 查询全部
来源：http://af.9csxet.cn

SELECT * FROM users;
来源：http://qh.9csxet.cn

[Q16] 查询指定列
来源：http://hw.huanxung.cn

SELECT id, name FROM users;
来源：http://cs.hahajie.cn

[Q17] 条件查询
来源：http://sg.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uv.panjiajie.cn

[Q18] 模糊匹配
来源：http://zv.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://la.bookmarksfly.cn

[Q19] 范围查询
来源：http://om.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qf.hnjuh.cn

[Q20] IN 列表
来源：http://ff.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iy.huixiangedu.cn

[Q21] 空值判断
来源：http://eu.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fd.huixinmuqiang.cn

[Q22] 排序
来源：http://cn.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hb.9csxet.cn

[Q23] 分页
来源：http://sw.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xh.huanxung.cn

[Q24] 去重
来源：http://dv.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ro.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://nc.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xn.panjiajie.cn

[Q26] 计数
来源：http://le.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://px.chemitech.net.cn

[Q27] 条件计数
来源：http://bn.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fs.huanxung.cn

[Q28] 求和与平均
来源：http://mm.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mb.hahajie.cn

[Q29] 最大最小值
来源：http://sx.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tn.gzmigu.cn

[Q30] 分组统计
来源：http://wj.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xn.nicolike.cn

[Q31] 分组后过滤
来源：http://ub.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tz.521024.cn

[Q32] 分组拼接字符串
来源：http://zn.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hr.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kw.huanxung.cn

[Q33] 多列分组
来源：http://xg.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://it.muxihuayi.cn

[Q34] 每组取第一条
来源：http://hd.szsharing.cn

SELECT * FROM (
来源：http://st.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ot.lnxyls.cn

) t WHERE rn = 1;
来源：http://us.yuexingan06.cn

[Q35] 内连接
来源：http://uf.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ea.gzmigu.cn

[Q36] 左连接
来源：http://mi.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bh.hnjuh.cn

[Q37] 右连接
来源：http://gw.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oi.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mh.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xf.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://mv.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bj.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hr.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wb.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lj.panjiajie.cn

[Q41] 多表连接
来源：http://wg.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fy.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://mu.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://mz.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://lt.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://ex.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yv.gzmigu.cn

[Q43] 标量子查询
来源：http://kv.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yg.huixiangedu.cn

[Q44] IN 子查询
来源：http://nj.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ve.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://ll.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zh.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ew.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wn.521024.cn

[Q47] 与平均值比较
来源：http://ar.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zy.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://if.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tu.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://wv.shxzskj.cn

[Q49] 更新单行
来源：http://cf.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bi.jctech888.com.cn

[Q50] 批量更新
来源：http://os.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pt.9csxet.cn

[Q51] 用子查询更新
来源：http://nj.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ek.shxzskj.cn

[Q52] 删除指定行
来源：http://wa.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://cg.huixiangedu.cn

[Q53] 按条件删除
来源：http://dg.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tp.huanxung.cn

[Q54] 清空表
来源：http://ru.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://ds.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://pe.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rl.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://xa.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nl.asd995.cn

[Q57] 行号
来源：http://yw.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iv.jctech888.com.cn

[Q58] 累计求和
来源：http://rr.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lh.haigaiapp.cn

[Q59] 分组内累计
来源：http://hd.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zf.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://wb.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pa.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bg.huixiangedu.cn

[Q61] 移动平均
来源：http://ry.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://av.jctech888.com.cn

[Q62] 分组占比
来源：http://is.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kw.colortex.cn

[Q63] 开启事务
来源：http://sp.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ep.yuexingan06.cn

[Q64] 提交事务
来源：http://my.yuexingan06.cn

COMMIT;
来源：http://wx.colortex.cn

[Q65] 回滚事务
来源：http://ae.shxzskj.cn

ROLLBACK;
来源：http://ty.521024.cn

[Q66] 行锁查询
来源：http://hn.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kk.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://iv.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vn.huixiangedu.cn

[Q68] 保存点
来源：http://xd.shtwfgs.cn

SAVEPOINT sp1;
来源：http://td.huanxung.cn

ROLLBACK TO sp1;
来源：http://kx.yuexingan06.cn

[Q69] 查看执行计划
来源：http://gn.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gf.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://oq.gzmigu.cn

ANALYZE TABLE users;
来源：http://ty.hahajie.cn

[Q71] 查看建表语句
来源：http://ez.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hh.bjjhwx.cn

[Q72] 查看索引
来源：http://bs.521024.cn

SHOW INDEX FROM users;
来源：http://yl.muxihuayi.cn

[Q73] 查看表状态
来源：http://vs.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rm.newstarts.cn

[Q74] 强制使用索引
来源：http://fa.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ol.huanxung.cn

[Q75] 日期格式化
来源：http://kh.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ky.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vg.bookmarksfly.cn

[Q76] 按天统计
来源：http://kd.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qw.nszjky.cn

[Q77] 时间加减
来源：http://xy.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ci.lnxyls.cn

[Q78] 当前时间
来源：http://wl.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://di.szxytkj.cn

[Q79] 字符串拼接
来源：http://dq.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gf.huanxung.cn

[Q80] 字符串截取
来源：http://rj.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qh.shxzukj.cn

[Q81] 字符串替换
来源：http://ak.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://du.521024.cn

[Q82] 字符长度与字节长度
来源：http://yr.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xj.newstarts.cn

[Q83] 大小写转换
来源：http://nb.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eu.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://sq.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://pi.szsharing.cn

[Q85] 数值取整
来源：http://oa.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jv.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://wz.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jo.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://bh.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qk.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://wp.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ov.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lg.9csxet.cn

[Q89] 判断表是否存在
来源：http://or.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qh.shxzukj.cn

[Q90] 生成序号列
来源：http://qe.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ei.szsharing.cn

================================================================================
来源：http://mh.bjjhwx.cn

R. Bash 专题
来源：http://jx.szxytkj.cn

================================================================================
来源：http://fd.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://cg.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://zx.jctech888.com.cn

set -euo pipefail
来源：http://iu.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://ib.szxytkj.cn

name="Tom"; echo "$name"
来源：http://gy.yuexingan06.cn

[R03] 只读变量
来源：http://jl.huanxung.cn

readonly PI=3.14
来源：http://qp.chemitech.net.cn

[R04] 位置参数
来源：http://cc.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wr.muxihuayi.cn

[R05] 参数默认值
来源：http://xw.jianghongdianzi.cn

name="${1:-default}"
来源：http://cr.asd995.cn

[R06] 判断命令是否存在
来源：http://lj.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zf.hahajie.cn

[R07] if 判断文件
来源：http://me.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mn.chemitech.net.cn

[R08] 数值比较
来源：http://wf.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ls.huixinmuqiang.cn

[R09] 字符串比较
来源：http://ot.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xz.chemitech.net.cn

[R10] 正则匹配
来源：http://na.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wb.newstarts.cn

[R11] case 多分支
来源：http://eo.yuntaijiaju.cn

case "$1" in
来源：http://qn.521024.cn

start) echo "启动" ;;
来源：http://fn.szxytkj.cn

stop)  echo "停止" ;;
来源：http://vv.colortex.cn

*)     echo "未知命令" ;;
来源：http://jp.bookmarksfly.cn


<!-- 参考信息 -->