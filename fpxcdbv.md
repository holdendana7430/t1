代发 wailian999

[P01] 生成 UUID
来源：http://hh.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://bh.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kp.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ng.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://pq.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://tw.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://kv.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://vy.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://ov.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://rd.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://au.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://be.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ka.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xz.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nf.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vk.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bz.hnjuh.cn

[P03] 生成短随机字符串
来源：http://pk.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sn.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sr.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vv.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gw.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://as.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vg.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gs.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xs.hnjuh.cn

[P04] 求长度
来源：http://de.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nb.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sq.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ji.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yw.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://rv.hahajie.cn

Go:   len(arr);  len(m)
来源：http://rt.9csxet.cn

Ruby: x.length;  x.size
来源：http://pr.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ge.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://rb.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://el.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mg.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zg.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gj.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vp.huixiangedu.cn

Ruby: a == b
来源：http://jl.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mr.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wc.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qs.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://mi.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://br.shxzskj.cn

TS:   if (x == null) {}
来源：http://cu.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qg.asd995.cn

Go:   if x == nil {}
来源：http://qi.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sk.lnxyls.cn

C#:   if (x is null) {}
来源：http://fi.bookmarksfly.cn

[P07] 防抖与节流
来源：http://vo.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rb.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://aa.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dk.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://st.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pz.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://st.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kz.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ag.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://rd.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ex.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://um.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rx.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uu.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hx.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pb.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uo.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zn.haigaiapp.cn

================================================================================
来源：http://zz.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zc.yuexingan06.cn

================================================================================
来源：http://qw.newstarts.cn

[Q01] 创建表
来源：http://wa.bjjhwx.cn

CREATE TABLE users (
来源：http://bm.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fi.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://kd.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://rm.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rx.gzmigu.cn

);
来源：http://bv.newstarts.cn

[Q02] 创建带外键的表
来源：http://so.yuexingan06.cn

CREATE TABLE orders (
来源：http://zg.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yp.huanxung.cn

user_id INT NOT NULL,
来源：http://wc.colortex.cn

amount DECIMAL(10, 2),
来源：http://xg.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://on.huixinmuqiang.cn

);
来源：http://rf.haigaiapp.cn

[Q03] 增加列
来源：http://pz.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mi.shxzukj.cn

[Q04] 修改列类型
来源：http://ok.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tq.521024.cn

[Q05] 重命名列
来源：http://go.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ho.hahajie.cn

[Q06] 删除列
来源：http://dq.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://et.jctech888.com.cn

[Q07] 删除表
来源：http://si.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://qd.huixiangedu.cn

[Q08] 创建普通索引
来源：http://bw.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://do.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://ap.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ew.wgjwhj.cn

[Q10] 插入单行
来源：http://bs.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://su.521024.cn

[Q11] 一次插入多行
来源：http://hn.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ut.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://vs.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qt.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gq.shxzukj.cn

[Q13] 忽略重复插入
来源：http://gc.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gk.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://fw.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ri.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wk.jianghongdianzi.cn

[Q15] 查询全部
来源：http://pm.panjiajie.cn

SELECT * FROM users;
来源：http://pt.szxytkj.cn

[Q16] 查询指定列
来源：http://cm.9csxet.cn

SELECT id, name FROM users;
来源：http://fc.newstarts.cn

[Q17] 条件查询
来源：http://tt.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nb.yuexingan06.cn

[Q18] 模糊匹配
来源：http://eu.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://of.huanxung.cn

[Q19] 范围查询
来源：http://ih.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ul.szxytkj.cn

[Q20] IN 列表
来源：http://os.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tm.colortex.cn

[Q21] 空值判断
来源：http://bd.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jl.huanxung.cn

[Q22] 排序
来源：http://gr.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://px.bookmarksfly.cn

[Q23] 分页
来源：http://qw.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ln.szsharing.cn

[Q24] 去重
来源：http://kc.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://mn.shxzskj.cn

[Q25] 只取前 N 条
来源：http://df.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ow.yuntaijiaju.cn

[Q26] 计数
来源：http://wy.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://ze.jctech888.com.cn

[Q27] 条件计数
来源：http://bx.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ev.panjiajie.cn

[Q28] 求和与平均
来源：http://xq.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dv.chemitech.net.cn

[Q29] 最大最小值
来源：http://nv.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wj.hnjuh.cn

[Q30] 分组统计
来源：http://dh.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ss.haigaiapp.cn

[Q31] 分组后过滤
来源：http://wh.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://av.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://pl.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qf.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pe.colortex.cn

[Q33] 多列分组
来源：http://vi.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ii.colortex.cn

[Q34] 每组取第一条
来源：http://cg.bjjhwx.cn

SELECT * FROM (
来源：http://oj.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ap.nszjky.cn

) t WHERE rn = 1;
来源：http://us.huixinmuqiang.cn

[Q35] 内连接
来源：http://sb.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://so.shxzskj.cn

[Q36] 左连接
来源：http://us.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vc.colortex.cn

[Q37] 右连接
来源：http://wt.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xp.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xq.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://os.colortex.cn

[Q39] 自连接（查上下级）
来源：http://hl.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bq.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ax.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ry.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gb.muxihuayi.cn

[Q41] 多表连接
来源：http://ny.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://aq.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://zs.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://zw.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://vj.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://da.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zx.newstarts.cn

[Q43] 标量子查询
来源：http://dj.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yj.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://wp.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wr.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://cg.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gq.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cd.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ex.wgjwhj.cn

[Q47] 与平均值比较
来源：http://kx.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wq.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://ln.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qr.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://yh.huanxung.cn

[Q49] 更新单行
来源：http://gh.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sd.bookmarksfly.cn

[Q50] 批量更新
来源：http://xl.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://az.hahajie.cn

[Q51] 用子查询更新
来源：http://es.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ou.newstarts.cn

[Q52] 删除指定行
来源：http://mz.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://zs.521024.cn

[Q53] 按条件删除
来源：http://gp.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ul.521024.cn

[Q54] 清空表
来源：http://lr.nicolike.cn

TRUNCATE TABLE logs;
来源：http://pq.9csxet.cn

[Q55] 排名（并列占位）
来源：http://oo.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jj.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://uc.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dp.panjiajie.cn

[Q57] 行号
来源：http://nm.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lc.wgjwhj.cn

[Q58] 累计求和
来源：http://to.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pl.hahajie.cn

[Q59] 分组内累计
来源：http://hf.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xo.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://mq.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lj.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cn.yuntaijiaju.cn

[Q61] 移动平均
来源：http://ai.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ns.jianghongdianzi.cn

[Q62] 分组占比
来源：http://cf.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://br.panjiajie.cn

[Q63] 开启事务
来源：http://fo.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kb.szsharing.cn

[Q64] 提交事务
来源：http://fx.jctech888.com.cn

COMMIT;
来源：http://ew.panjiajie.cn

[Q65] 回滚事务
来源：http://ai.yuexingan06.cn

ROLLBACK;
来源：http://ty.nicolike.cn

[Q66] 行锁查询
来源：http://vq.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dj.nicolike.cn

[Q67] 设置隔离级别
来源：http://wm.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xy.gzmigu.cn

[Q68] 保存点
来源：http://fk.hnjuh.cn

SAVEPOINT sp1;
来源：http://ky.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://ac.colortex.cn

[Q69] 查看执行计划
来源：http://xx.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nq.wgjwhj.cn

[Q70] 更新统计信息
来源：http://iq.hnjuh.cn

ANALYZE TABLE users;
来源：http://mi.colortex.cn

[Q71] 查看建表语句
来源：http://ph.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yi.lnxyls.cn

[Q72] 查看索引
来源：http://od.szxytkj.cn

SHOW INDEX FROM users;
来源：http://oo.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://fe.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zm.lnxyls.cn

[Q74] 强制使用索引
来源：http://nx.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qj.haigaiapp.cn

[Q75] 日期格式化
来源：http://di.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gl.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vy.colortex.cn

[Q76] 按天统计
来源：http://pl.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ss.asd995.cn

[Q77] 时间加减
来源：http://nt.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zy.hahajie.cn

[Q78] 当前时间
来源：http://gx.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iw.shxzukj.cn

[Q79] 字符串拼接
来源：http://wt.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bs.wgjwhj.cn

[Q80] 字符串截取
来源：http://yz.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wv.newstarts.cn

[Q81] 字符串替换
来源：http://io.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ad.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://ro.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ui.szsharing.cn

[Q83] 大小写转换
来源：http://rc.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xq.huanxung.cn

[Q84] 去除首尾空格
来源：http://iv.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ve.yuntaijiaju.cn

[Q85] 数值取整
来源：http://sh.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pv.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://hw.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lq.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://yg.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nl.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://pt.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jx.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pe.shxzskj.cn

[Q89] 判断表是否存在
来源：http://mg.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://su.yuexingan06.cn

[Q90] 生成序号列
来源：http://kd.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rw.shtwfgs.cn

================================================================================
来源：http://kj.haigaiapp.cn

R. Bash 专题
来源：http://et.gzmigu.cn

================================================================================
来源：http://vz.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://nk.nszjky.cn

#!/usr/bin/env bash
来源：http://xp.asd995.cn

set -euo pipefail
来源：http://ji.gzmigu.cn

[R02] 变量赋值与使用
来源：http://bx.hnjuh.cn

name="Tom"; echo "$name"
来源：http://oz.haigaiapp.cn

[R03] 只读变量
来源：http://bh.bjjhwx.cn

readonly PI=3.14
来源：http://gq.shxzskj.cn

[R04] 位置参数
来源：http://ey.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rt.lnxyls.cn

[R05] 参数默认值
来源：http://go.gzmigu.cn

name="${1:-default}"
来源：http://zh.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://uv.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wg.hahajie.cn

[R07] if 判断文件
来源：http://hz.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vs.huanxung.cn

[R08] 数值比较
来源：http://dz.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sm.shxzukj.cn

[R09] 字符串比较
来源：http://sz.bjjhwx.cn


<!-- 参考信息 -->