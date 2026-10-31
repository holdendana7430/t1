代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dl.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://up.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rp.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kg.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oq.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dc.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://mo.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qh.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://in.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kn.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ts.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ud.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rm.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xl.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fc.huixinmuqiang.cn

[P04] 求长度
来源：http://qw.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://np.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cr.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wk.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dz.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://lx.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://mb.szsharing.cn

Ruby: x.length;  x.size
来源：http://xr.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fb.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://ao.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ox.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rw.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ad.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qi.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ax.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jh.lnxyls.cn

Ruby: a == b
来源：http://kh.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lz.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ym.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://na.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://zn.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://in.shxzukj.cn

TS:   if (x == null) {}
来源：http://at.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yc.szsharing.cn

Go:   if x == nil {}
来源：http://fc.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tt.jctech888.com.cn

C#:   if (x is null) {}
来源：http://cl.muxihuayi.cn

[P07] 防抖与节流
来源：http://sz.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aj.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://wg.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vm.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ud.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://od.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hg.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vx.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bs.521024.cn

[P08] 处理浮点精度问题
来源：http://fw.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dh.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zz.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cj.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sd.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rs.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zl.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jf.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oh.nszjky.cn

================================================================================
来源：http://iu.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eq.huixiangedu.cn

================================================================================
来源：http://ss.9csxet.cn

[Q01] 创建表
来源：http://ti.haigaiapp.cn

CREATE TABLE users (
来源：http://tx.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yv.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://hr.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://in.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wj.shxzskj.cn

);
来源：http://du.shxzukj.cn

[Q02] 创建带外键的表
来源：http://rp.shxzukj.cn

CREATE TABLE orders (
来源：http://mj.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yl.muxihuayi.cn

user_id INT NOT NULL,
来源：http://zc.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://il.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fa.bjjhwx.cn

);
来源：http://rf.shxzskj.cn

[Q03] 增加列
来源：http://st.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://il.panjiajie.cn

[Q04] 修改列类型
来源：http://oj.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mz.jctech888.com.cn

[Q05] 重命名列
来源：http://tn.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ei.jianghongdianzi.cn

[Q06] 删除列
来源：http://rw.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sw.panjiajie.cn

[Q07] 删除表
来源：http://gl.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://ae.nicolike.cn

[Q08] 创建普通索引
来源：http://vz.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zx.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://ng.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gi.huixinmuqiang.cn

[Q10] 插入单行
来源：http://qo.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ul.muxihuayi.cn

[Q11] 一次插入多行
来源：http://on.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wl.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://yg.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://os.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fl.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://ty.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rf.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://gi.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fi.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qz.szsharing.cn

[Q15] 查询全部
来源：http://br.yuntaijiaju.cn

SELECT * FROM users;
来源：http://do.huixiangedu.cn

[Q16] 查询指定列
来源：http://wt.nicolike.cn

SELECT id, name FROM users;
来源：http://qn.bjjhwx.cn

[Q17] 条件查询
来源：http://ob.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cy.colortex.cn

[Q18] 模糊匹配
来源：http://qw.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aw.bjjhwx.cn

[Q19] 范围查询
来源：http://wy.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eb.huanxung.cn

[Q20] IN 列表
来源：http://ii.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gs.muxihuayi.cn

[Q21] 空值判断
来源：http://xv.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hj.jctech888.com.cn

[Q22] 排序
来源：http://wf.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mo.haigaiapp.cn

[Q23] 分页
来源：http://eh.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bs.szsharing.cn

[Q24] 去重
来源：http://ku.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://ul.nicolike.cn

[Q25] 只取前 N 条
来源：http://qv.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sn.hnjuh.cn

[Q26] 计数
来源：http://up.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://wx.szxytkj.cn

[Q27] 条件计数
来源：http://vj.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bt.panjiajie.cn

[Q28] 求和与平均
来源：http://of.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dx.huixiangedu.cn

[Q29] 最大最小值
来源：http://tp.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ui.bjjhwx.cn

[Q30] 分组统计
来源：http://du.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ld.hahajie.cn

[Q31] 分组后过滤
来源：http://ey.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ed.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://hl.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wk.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ap.muxihuayi.cn

[Q33] 多列分组
来源：http://mj.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ui.newstarts.cn

[Q34] 每组取第一条
来源：http://fm.szxytkj.cn

SELECT * FROM (
来源：http://us.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ne.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://dx.shxzskj.cn

[Q35] 内连接
来源：http://fu.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rj.hnjuh.cn

[Q36] 左连接
来源：http://ri.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ov.colortex.cn

[Q37] 右连接
来源：http://bs.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rv.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qs.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kd.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://fo.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gt.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jk.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gb.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ij.huixinmuqiang.cn

[Q41] 多表连接
来源：http://yf.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ah.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://wp.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://sj.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://oh.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://rj.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gc.szxytkj.cn

[Q43] 标量子查询
来源：http://fl.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pd.9csxet.cn

[Q44] IN 子查询
来源：http://vm.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mg.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://cq.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iv.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zg.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mb.nicolike.cn

[Q47] 与平均值比较
来源：http://vv.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://py.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://ul.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oq.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://uv.nicolike.cn

[Q49] 更新单行
来源：http://zu.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ei.wgjwhj.cn

[Q50] 批量更新
来源：http://yl.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yr.newstarts.cn

[Q51] 用子查询更新
来源：http://us.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pf.shxzukj.cn

[Q52] 删除指定行
来源：http://ts.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://fa.nicolike.cn

[Q53] 按条件删除
来源：http://hx.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ng.yuexingan06.cn

[Q54] 清空表
来源：http://tr.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://wk.asd995.cn

[Q55] 排名（并列占位）
来源：http://th.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wr.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://yc.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nz.jianghongdianzi.cn

[Q57] 行号
来源：http://nr.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oh.yuntaijiaju.cn

[Q58] 累计求和
来源：http://up.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fj.haigaiapp.cn

[Q59] 分组内累计
来源：http://qb.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hl.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://vg.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mo.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ou.jctech888.com.cn

[Q61] 移动平均
来源：http://nt.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kc.newstarts.cn

[Q62] 分组占比
来源：http://zg.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cl.shxzskj.cn

[Q63] 开启事务
来源：http://ot.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://la.huixinmuqiang.cn

[Q64] 提交事务
来源：http://cu.yuntaijiaju.cn

COMMIT;
来源：http://mw.9csxet.cn

[Q65] 回滚事务
来源：http://os.nszjky.cn

ROLLBACK;
来源：http://gl.colortex.cn

[Q66] 行锁查询
来源：http://wv.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rv.nicolike.cn

[Q67] 设置隔离级别
来源：http://fw.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vq.shxzukj.cn

[Q68] 保存点
来源：http://lc.nicolike.cn

SAVEPOINT sp1;
来源：http://uy.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://lk.nicolike.cn

[Q69] 查看执行计划
来源：http://bg.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ea.newstarts.cn

[Q70] 更新统计信息
来源：http://yc.asd995.cn

ANALYZE TABLE users;
来源：http://um.hahajie.cn

[Q71] 查看建表语句
来源：http://ax.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vs.bjjhwx.cn

[Q72] 查看索引
来源：http://dp.asd995.cn

SHOW INDEX FROM users;
来源：http://in.colortex.cn

[Q73] 查看表状态
来源：http://rx.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ta.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://qh.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pz.nicolike.cn

[Q75] 日期格式化
来源：http://bm.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zy.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pz.nicolike.cn

[Q76] 按天统计
来源：http://aw.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://al.asd995.cn

[Q77] 时间加减
来源：http://sv.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yp.huixiangedu.cn

[Q78] 当前时间
来源：http://de.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ww.muxihuayi.cn

[Q79] 字符串拼接
来源：http://ws.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xu.asd995.cn

[Q80] 字符串截取
来源：http://eg.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sy.shxzukj.cn

[Q81] 字符串替换
来源：http://yh.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mm.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://pm.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kb.muxihuayi.cn

[Q83] 大小写转换
来源：http://tf.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pg.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://zw.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://be.nicolike.cn

[Q85] 数值取整
来源：http://cm.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fs.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://yz.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://al.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://jv.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gq.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://rk.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cx.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ag.9csxet.cn

[Q89] 判断表是否存在
来源：http://lo.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qz.hnjuh.cn

[Q90] 生成序号列
来源：http://zr.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pa.asd995.cn

================================================================================
来源：http://ss.yuntaijiaju.cn

R. Bash 专题
来源：http://eq.lnxyls.cn

================================================================================
来源：http://xq.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://bz.muxihuayi.cn

#!/usr/bin/env bash
来源：http://pp.huanxung.cn

set -euo pipefail
来源：http://bq.szsharing.cn

[R02] 变量赋值与使用
来源：http://la.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ej.jctech888.com.cn

[R03] 只读变量
来源：http://ci.jctech888.com.cn

readonly PI=3.14
来源：http://us.nszjky.cn

[R04] 位置参数
来源：http://we.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://is.gzmigu.cn

[R05] 参数默认值
来源：http://rl.gzmigu.cn

name="${1:-default}"
来源：http://ua.nicolike.cn

[R06] 判断命令是否存在
来源：http://yh.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pq.shxzukj.cn

[R07] if 判断文件
来源：http://lb.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uz.jctech888.com.cn

[R08] 数值比较
来源：http://xg.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tu.shtwfgs.cn

[R09] 字符串比较
来源：http://np.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oo.colortex.cn

[R10] 正则匹配
来源：http://os.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nv.bjjhwx.cn

[R11] case 多分支
来源：http://wk.huanxung.cn

case "$1" in
来源：http://dp.9csxet.cn

start) echo "启动" ;;
来源：http://mh.asd995.cn

stop)  echo "停止" ;;
来源：http://cx.szsharing.cn

*)     echo "未知命令" ;;
来源：http://tf.gzmigu.cn

esac
来源：http://md.521024.cn

[R12] for 遍历文件
来源：http://lt.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://rb.hahajie.cn

[R13] for 计数循环
来源：http://fp.chemitech.net.cn


<!-- 参考信息 -->