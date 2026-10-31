代发 wailian999

TS:   // child_process / cluster 模块
来源：http://ew.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zy.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jp.bjjhwx.cn

Ruby: // fork 块
来源：http://ed.shxzskj.cn

C#:   Parallel.For
来源：http://qp.yuexingan06.cn

================================================================================
来源：http://nd.bjjhwx.cn

P. 常用工具函数
来源：http://nf.hahajie.cn

================================================================================
来源：http://rd.hnjuh.cn

[P01] 生成 UUID
来源：http://ky.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://ix.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xz.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://nj.hahajie.cn

TS:   crypto.randomUUID()
来源：http://ec.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://tj.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://iu.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://fc.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://om.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://ol.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://os.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ky.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qr.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dq.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ww.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zy.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xp.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ny.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://si.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ao.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ss.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ov.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ue.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mq.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hy.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://es.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tf.9csxet.cn

[P04] 求长度
来源：http://bp.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://br.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hc.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nd.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dj.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://vv.nszjky.cn

Go:   len(arr);  len(m)
来源：http://ro.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://sx.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ay.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://qh.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ip.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lz.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hb.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sz.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vl.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eb.huixiangedu.cn

Ruby: a == b
来源：http://ua.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aq.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zn.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tc.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://nr.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dg.hnjuh.cn

TS:   if (x == null) {}
来源：http://tw.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fp.yuexingan06.cn

Go:   if x == nil {}
来源：http://sy.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ho.szxytkj.cn

C#:   if (x is null) {}
来源：http://ws.lnxyls.cn

[P07] 防抖与节流
来源：http://dp.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yd.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://ez.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ko.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://og.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eb.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ai.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ax.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://kp.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pc.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qd.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ao.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qg.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ns.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zg.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aq.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://or.muxihuayi.cn

================================================================================
来源：http://kn.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vz.huanxung.cn

================================================================================
来源：http://gv.haigaiapp.cn

[Q01] 创建表
来源：http://jc.521024.cn

CREATE TABLE users (
来源：http://sv.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fi.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://az.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://ku.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sx.colortex.cn

);
来源：http://mh.gzmigu.cn

[Q02] 创建带外键的表
来源：http://kx.muxihuayi.cn

CREATE TABLE orders (
来源：http://aw.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xo.szsharing.cn

user_id INT NOT NULL,
来源：http://rd.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://hz.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ww.huixinmuqiang.cn

);
来源：http://gc.huixinmuqiang.cn

[Q03] 增加列
来源：http://hi.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cd.521024.cn

[Q04] 修改列类型
来源：http://hi.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gq.newstarts.cn

[Q05] 重命名列
来源：http://im.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://st.bookmarksfly.cn

[Q06] 删除列
来源：http://nx.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wn.gzmigu.cn

[Q07] 删除表
来源：http://os.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://ta.hahajie.cn

[Q08] 创建普通索引
来源：http://tm.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pf.newstarts.cn

[Q09] 创建唯一索引
来源：http://da.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://an.chemitech.net.cn

[Q10] 插入单行
来源：http://lx.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gh.szxytkj.cn

[Q11] 一次插入多行
来源：http://sg.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iz.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://jz.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://su.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bl.nicolike.cn

[Q13] 忽略重复插入
来源：http://uk.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hg.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://cz.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jo.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dt.gzmigu.cn

[Q15] 查询全部
来源：http://fe.bjjhwx.cn

SELECT * FROM users;
来源：http://kv.9csxet.cn

[Q16] 查询指定列
来源：http://bj.gzmigu.cn

SELECT id, name FROM users;
来源：http://cl.szxytkj.cn

[Q17] 条件查询
来源：http://qj.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://am.wgjwhj.cn

[Q18] 模糊匹配
来源：http://pv.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vz.yuntaijiaju.cn

[Q19] 范围查询
来源：http://yq.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yu.521024.cn

[Q20] IN 列表
来源：http://jn.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://er.yuexingan06.cn

[Q21] 空值判断
来源：http://rk.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fh.bjjhwx.cn

[Q22] 排序
来源：http://qk.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ge.shxzskj.cn

[Q23] 分页
来源：http://gx.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hs.shtwfgs.cn

[Q24] 去重
来源：http://rv.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://gu.hnjuh.cn

[Q25] 只取前 N 条
来源：http://kt.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nc.9csxet.cn

[Q26] 计数
来源：http://vg.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://nu.521024.cn

[Q27] 条件计数
来源：http://gc.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gj.jctech888.com.cn

[Q28] 求和与平均
来源：http://js.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kp.shtwfgs.cn

[Q29] 最大最小值
来源：http://hp.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://il.newstarts.cn

[Q30] 分组统计
来源：http://um.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dp.gzmigu.cn

[Q31] 分组后过滤
来源：http://zl.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vt.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://sg.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qr.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vp.jianghongdianzi.cn

[Q33] 多列分组
来源：http://kw.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rl.muxihuayi.cn

[Q34] 每组取第一条
来源：http://tm.wgjwhj.cn

SELECT * FROM (
来源：http://de.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mu.panjiajie.cn

) t WHERE rn = 1;
来源：http://ws.nicolike.cn

[Q35] 内连接
来源：http://ut.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gt.bjjhwx.cn

[Q36] 左连接
来源：http://sv.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fc.muxihuayi.cn

[Q37] 右连接
来源：http://ed.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nf.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ct.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mf.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://vp.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gx.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hh.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kw.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hh.gzmigu.cn

[Q41] 多表连接
来源：http://rz.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sy.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://ln.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://mh.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://ty.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://cc.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mv.yuexingan06.cn

[Q43] 标量子查询
来源：http://ut.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fg.521024.cn

[Q44] IN 子查询
来源：http://wz.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fg.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ru.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qz.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fg.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iy.521024.cn

[Q47] 与平均值比较
来源：http://wh.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ti.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://mi.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xs.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://rt.hahajie.cn

[Q49] 更新单行
来源：http://kt.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jg.colortex.cn

[Q50] 批量更新
来源：http://jy.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oe.huanxung.cn

[Q51] 用子查询更新
来源：http://em.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sg.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://oa.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://yt.521024.cn

[Q53] 按条件删除
来源：http://to.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qx.lnxyls.cn

[Q54] 清空表
来源：http://dx.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://dx.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://el.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ry.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://ey.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fx.huanxung.cn

[Q57] 行号
来源：http://ag.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vy.haigaiapp.cn

[Q58] 累计求和
来源：http://ml.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kw.asd995.cn

[Q59] 分组内累计
来源：http://zy.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zm.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://qv.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lz.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fo.colortex.cn

[Q61] 移动平均
来源：http://ck.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qa.jctech888.com.cn

[Q62] 分组占比
来源：http://ms.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fw.colortex.cn

[Q63] 开启事务
来源：http://ib.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sp.huixiangedu.cn

[Q64] 提交事务
来源：http://av.nszjky.cn

COMMIT;
来源：http://iy.wgjwhj.cn

[Q65] 回滚事务
来源：http://zo.nicolike.cn

ROLLBACK;
来源：http://qm.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://gc.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ub.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://yk.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dg.jianghongdianzi.cn

[Q68] 保存点
来源：http://ww.nszjky.cn

SAVEPOINT sp1;
来源：http://wf.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://tb.panjiajie.cn

[Q69] 查看执行计划
来源：http://xm.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yv.shxzukj.cn

[Q70] 更新统计信息
来源：http://lt.wgjwhj.cn

ANALYZE TABLE users;
来源：http://da.muxihuayi.cn

[Q71] 查看建表语句
来源：http://vl.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jk.shxzukj.cn

[Q72] 查看索引
来源：http://am.521024.cn

SHOW INDEX FROM users;
来源：http://pf.colortex.cn

[Q73] 查看表状态
来源：http://iw.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wj.huanxung.cn

[Q74] 强制使用索引
来源：http://hu.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ur.521024.cn

[Q75] 日期格式化
来源：http://dm.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hb.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zr.szxytkj.cn

[Q76] 按天统计
来源：http://pa.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yq.newstarts.cn

[Q77] 时间加减
来源：http://pq.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hb.shtwfgs.cn

[Q78] 当前时间
来源：http://dg.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vn.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://bf.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zp.gzmigu.cn

[Q80] 字符串截取
来源：http://qy.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tr.panjiajie.cn

[Q81] 字符串替换
来源：http://gl.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hb.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://sh.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vh.nicolike.cn

[Q83] 大小写转换
来源：http://sr.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cw.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://vm.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://ch.hahajie.cn

[Q85] 数值取整
来源：http://zo.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fs.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://ub.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uz.nszjky.cn

[Q87] JSON 字段做条件
来源：http://hs.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://po.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://en.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zd.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jd.szsharing.cn

[Q89] 判断表是否存在
来源：http://br.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nj.nicolike.cn

[Q90] 生成序号列
来源：http://mb.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rf.szsharing.cn

================================================================================
来源：http://yc.bookmarksfly.cn

R. Bash 专题
来源：http://pi.jctech888.com.cn

================================================================================
来源：http://rn.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://pl.shtwfgs.cn

#!/usr/bin/env bash
来源：http://gd.huanxung.cn

set -euo pipefail
来源：http://ag.shxzskj.cn

[R02] 变量赋值与使用
来源：http://dq.colortex.cn

name="Tom"; echo "$name"
来源：http://bb.szsharing.cn

[R03] 只读变量
来源：http://tr.yuexingan06.cn

readonly PI=3.14
来源：http://xu.szxytkj.cn

[R04] 位置参数
来源：http://cf.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cv.szxytkj.cn

[R05] 参数默认值
来源：http://yr.shxzskj.cn


<!-- 参考信息 -->