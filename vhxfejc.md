代发 wailian999

TS:   // child_process / cluster 模块
来源：http://tk.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hh.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gi.shxzskj.cn

Ruby: // fork 块
来源：http://zl.nszjky.cn

C#:   Parallel.For
来源：http://fl.hahajie.cn

================================================================================
来源：http://ub.newstarts.cn

P. 常用工具函数
来源：http://wr.jianghongdianzi.cn

================================================================================
来源：http://ol.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://wn.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://iv.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hi.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://te.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://qd.521024.cn

Java: UUID.randomUUID().toString()
来源：http://en.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://ze.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://ri.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://tu.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://et.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pg.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gq.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zf.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ym.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ny.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://js.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dv.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jh.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://bb.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lz.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nv.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wk.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nd.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://px.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rr.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xe.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ib.shtwfgs.cn

[P04] 求长度
来源：http://hh.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jv.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zq.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ae.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sv.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://mv.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://ds.huanxung.cn

Ruby: x.length;  x.size
来源：http://uu.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mc.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://bt.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://co.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yz.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qg.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lh.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yw.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cu.muxihuayi.cn

Ruby: a == b
来源：http://zc.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gg.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://az.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pt.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://qi.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ul.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://ba.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wb.huixiangedu.cn

Go:   if x == nil {}
来源：http://vo.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qu.gzmigu.cn

C#:   if (x is null) {}
来源：http://ap.szxytkj.cn

[P07] 防抖与节流
来源：http://kk.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lp.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://lh.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xe.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wi.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gp.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zg.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ys.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://td.asd995.cn

[P08] 处理浮点精度问题
来源：http://yd.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ln.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eh.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yg.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uj.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vy.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jx.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://go.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ro.521024.cn

================================================================================
来源：http://ed.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iw.szxytkj.cn

================================================================================
来源：http://ih.521024.cn

[Q01] 创建表
来源：http://zg.szxytkj.cn

CREATE TABLE users (
来源：http://ea.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sh.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://sh.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://vd.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nicolike.cn

);
来源：http://fk.nszjky.cn

[Q02] 创建带外键的表
来源：http://vx.bjjhwx.cn

CREATE TABLE orders (
来源：http://mm.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tn.gzmigu.cn

user_id INT NOT NULL,
来源：http://ua.huanxung.cn

amount DECIMAL(10, 2),
来源：http://zb.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ro.szxytkj.cn

);
来源：http://fw.muxihuayi.cn

[Q03] 增加列
来源：http://gp.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pe.muxihuayi.cn

[Q04] 修改列类型
来源：http://ns.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ps.nszjky.cn

[Q05] 重命名列
来源：http://hm.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zd.haigaiapp.cn

[Q06] 删除列
来源：http://ks.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mv.bjjhwx.cn

[Q07] 删除表
来源：http://lh.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://dh.colortex.cn

[Q08] 创建普通索引
来源：http://ro.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sa.nszjky.cn

[Q09] 创建唯一索引
来源：http://ie.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gf.panjiajie.cn

[Q10] 插入单行
来源：http://vj.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uq.jctech888.com.cn

[Q11] 一次插入多行
来源：http://xl.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ag.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://it.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yv.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pi.521024.cn

[Q13] 忽略重复插入
来源：http://fo.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kh.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://bd.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ps.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://st.asd995.cn

[Q15] 查询全部
来源：http://ce.szsharing.cn

SELECT * FROM users;
来源：http://js.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://en.jctech888.com.cn

SELECT id, name FROM users;
来源：http://vm.haigaiapp.cn

[Q17] 条件查询
来源：http://wy.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tw.bjjhwx.cn

[Q18] 模糊匹配
来源：http://xj.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hv.szxytkj.cn

[Q19] 范围查询
来源：http://ff.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xt.muxihuayi.cn

[Q20] IN 列表
来源：http://jq.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nu.panjiajie.cn

[Q21] 空值判断
来源：http://ol.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zk.jctech888.com.cn

[Q22] 排序
来源：http://wn.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ir.shxzskj.cn

[Q23] 分页
来源：http://oq.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pk.nicolike.cn

[Q24] 去重
来源：http://jc.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://ee.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://hy.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ry.lnxyls.cn

[Q26] 计数
来源：http://gr.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://pn.nszjky.cn

[Q27] 条件计数
来源：http://px.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jh.nszjky.cn

[Q28] 求和与平均
来源：http://dc.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dn.gzmigu.cn

[Q29] 最大最小值
来源：http://al.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://om.lnxyls.cn

[Q30] 分组统计
来源：http://ag.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pd.521024.cn

[Q31] 分组后过滤
来源：http://xm.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wb.9csxet.cn

[Q32] 分组拼接字符串
来源：http://cs.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kz.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ge.yuexingan06.cn

[Q33] 多列分组
来源：http://cl.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gf.9csxet.cn

[Q34] 每组取第一条
来源：http://nz.nszjky.cn

SELECT * FROM (
来源：http://xy.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sv.gzmigu.cn

) t WHERE rn = 1;
来源：http://qc.muxihuayi.cn

[Q35] 内连接
来源：http://vt.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lp.521024.cn

[Q36] 左连接
来源：http://hz.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hi.shtwfgs.cn

[Q37] 右连接
来源：http://bq.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pr.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ty.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yi.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://bq.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ja.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xc.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iw.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dy.huixiangedu.cn

[Q41] 多表连接
来源：http://bk.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gs.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://cp.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://xb.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://eq.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://vq.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zp.panjiajie.cn

[Q43] 标量子查询
来源：http://cj.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://he.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://dt.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://et.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://zy.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sb.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jg.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ju.nszjky.cn

[Q47] 与平均值比较
来源：http://jx.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rk.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://xd.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ue.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://eq.yuntaijiaju.cn

[Q49] 更新单行
来源：http://dd.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://me.wgjwhj.cn

[Q50] 批量更新
来源：http://th.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ht.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://zl.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://od.9csxet.cn

[Q52] 删除指定行
来源：http://wv.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://so.wgjwhj.cn

[Q53] 按条件删除
来源：http://ll.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fs.yuexingan06.cn

[Q54] 清空表
来源：http://uw.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ol.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ue.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uy.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://fn.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://st.wgjwhj.cn

[Q57] 行号
来源：http://dd.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pw.huanxung.cn

[Q58] 累计求和
来源：http://bl.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mf.newstarts.cn

[Q59] 分组内累计
来源：http://yp.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yb.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://xa.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xp.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bi.huixinmuqiang.cn

[Q61] 移动平均
来源：http://nm.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lo.haigaiapp.cn

[Q62] 分组占比
来源：http://zd.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ae.shtwfgs.cn

[Q63] 开启事务
来源：http://og.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zu.haigaiapp.cn

[Q64] 提交事务
来源：http://bg.521024.cn

COMMIT;
来源：http://xu.nszjky.cn

[Q65] 回滚事务
来源：http://cd.bjjhwx.cn

ROLLBACK;
来源：http://ai.muxihuayi.cn

[Q66] 行锁查询
来源：http://eu.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tm.521024.cn

[Q67] 设置隔离级别
来源：http://xo.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lx.newstarts.cn

[Q68] 保存点
来源：http://za.nszjky.cn

SAVEPOINT sp1;
来源：http://kr.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ez.colortex.cn

[Q69] 查看执行计划
来源：http://sn.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yf.jctech888.com.cn

[Q70] 更新统计信息
来源：http://fu.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://bd.muxihuayi.cn

[Q71] 查看建表语句
来源：http://rk.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://th.hnjuh.cn

[Q72] 查看索引
来源：http://ee.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://du.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://vl.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zm.nicolike.cn

[Q74] 强制使用索引
来源：http://ia.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tb.nicolike.cn

[Q75] 日期格式化
来源：http://ka.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://es.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ao.bookmarksfly.cn

[Q76] 按天统计
来源：http://du.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hd.muxihuayi.cn

[Q77] 时间加减
来源：http://lj.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dc.szxytkj.cn

[Q78] 当前时间
来源：http://nx.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lp.muxihuayi.cn

[Q79] 字符串拼接
来源：http://gz.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://su.chemitech.net.cn

[Q80] 字符串截取
来源：http://jc.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ni.chemitech.net.cn

[Q81] 字符串替换
来源：http://jc.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iq.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://us.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kl.jctech888.com.cn

[Q83] 大小写转换
来源：http://as.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rn.nicolike.cn

[Q84] 去除首尾空格
来源：http://nz.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://kc.yuntaijiaju.cn

[Q85] 数值取整
来源：http://eh.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://or.asd995.cn

[Q86] 读取 JSON 字段
来源：http://xz.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ix.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://nk.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wr.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://uf.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uq.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zm.szxytkj.cn

[Q89] 判断表是否存在
来源：http://po.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yf.szxytkj.cn

[Q90] 生成序号列
来源：http://rv.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rz.bookmarksfly.cn

================================================================================
来源：http://nh.panjiajie.cn

R. Bash 专题
来源：http://tl.colortex.cn

================================================================================
来源：http://ug.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://mb.9csxet.cn

#!/usr/bin/env bash
来源：http://db.chemitech.net.cn

set -euo pipefail
来源：http://xt.nszjky.cn

[R02] 变量赋值与使用
来源：http://nn.9csxet.cn

name="Tom"; echo "$name"
来源：http://ak.asd995.cn

[R03] 只读变量
来源：http://ze.9csxet.cn

readonly PI=3.14
来源：http://jy.yuexingan06.cn

[R04] 位置参数
来源：http://qx.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ft.haigaiapp.cn

[R05] 参数默认值
来源：http://yo.nszjky.cn


<!-- 参考信息 -->