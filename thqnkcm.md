代发 wailian999

[O06] 使用进程池
来源：http://ka.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gf.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ni.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://vd.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://gl.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bd.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bq.shxzskj.cn

Ruby: // fork 块
来源：http://ul.panjiajie.cn

C#:   Parallel.For
来源：http://qg.hahajie.cn

================================================================================
来源：http://qx.521024.cn

P. 常用工具函数
来源：http://zv.hahajie.cn

================================================================================
来源：http://ek.yuexingan06.cn

[P01] 生成 UUID
来源：http://og.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://yb.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gw.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://pq.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://uj.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://di.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://xk.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://uu.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://cr.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://vk.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cn.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ky.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oy.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dd.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uu.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ap.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zl.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ok.szxytkj.cn

[P03] 生成短随机字符串
来源：http://nf.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://el.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bl.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iy.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xf.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lf.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fn.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bd.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tu.hnjuh.cn

[P04] 求长度
来源：http://qc.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vz.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pt.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oh.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://kg.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://yu.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://ht.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qc.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://an.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jk.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mx.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xm.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pn.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wk.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ds.huixiangedu.cn

Ruby: a == b
来源：http://lf.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fa.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vj.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hv.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://tz.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pp.chemitech.net.cn

TS:   if (x == null) {}
来源：http://gz.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dx.panjiajie.cn

Go:   if x == nil {}
来源：http://oh.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ma.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ah.lnxyls.cn

[P07] 防抖与节流
来源：http://om.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hn.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ot.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vo.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nm.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fs.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ak.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://of.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sm.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://ju.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://at.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rg.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ka.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cx.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ft.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vl.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yb.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lq.colortex.cn

================================================================================
来源：http://ln.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pt.chemitech.net.cn

================================================================================
来源：http://iy.asd995.cn

[Q01] 创建表
来源：http://ls.shxzskj.cn

CREATE TABLE users (
来源：http://wm.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mx.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ro.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://nt.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ke.jctech888.com.cn

);
来源：http://np.asd995.cn

[Q02] 创建带外键的表
来源：http://qy.muxihuayi.cn

CREATE TABLE orders (
来源：http://cl.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yy.szsharing.cn

user_id INT NOT NULL,
来源：http://ye.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://zj.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dp.huixinmuqiang.cn

);
来源：http://ua.yuntaijiaju.cn

[Q03] 增加列
来源：http://tu.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://st.muxihuayi.cn

[Q04] 修改列类型
来源：http://bw.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pt.bookmarksfly.cn

[Q05] 重命名列
来源：http://mc.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://go.hnjuh.cn

[Q06] 删除列
来源：http://pq.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lj.chemitech.net.cn

[Q07] 删除表
来源：http://vo.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://tu.huixiangedu.cn

[Q08] 创建普通索引
来源：http://dq.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ye.521024.cn

[Q09] 创建唯一索引
来源：http://ap.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jd.bjjhwx.cn

[Q10] 插入单行
来源：http://jo.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rd.yuexingan06.cn

[Q11] 一次插入多行
来源：http://fx.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ar.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ra.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yi.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ea.szsharing.cn

[Q13] 忽略重复插入
来源：http://ml.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pr.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://qc.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://to.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sx.bookmarksfly.cn

[Q15] 查询全部
来源：http://bi.asd995.cn

SELECT * FROM users;
来源：http://sk.jctech888.com.cn

[Q16] 查询指定列
来源：http://cc.panjiajie.cn

SELECT id, name FROM users;
来源：http://sb.521024.cn

[Q17] 条件查询
来源：http://pg.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jq.hahajie.cn

[Q18] 模糊匹配
来源：http://to.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ig.haigaiapp.cn

[Q19] 范围查询
来源：http://bd.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ze.bjjhwx.cn

[Q20] IN 列表
来源：http://df.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zw.bjjhwx.cn

[Q21] 空值判断
来源：http://gv.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zd.shxzukj.cn

[Q22] 排序
来源：http://nv.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cr.hahajie.cn

[Q23] 分页
来源：http://xw.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vz.haigaiapp.cn

[Q24] 去重
来源：http://vc.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://zu.hnjuh.cn

[Q25] 只取前 N 条
来源：http://jv.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ga.shtwfgs.cn

[Q26] 计数
来源：http://nr.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://mm.shxzukj.cn

[Q27] 条件计数
来源：http://rf.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rv.jctech888.com.cn

[Q28] 求和与平均
来源：http://er.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wx.haigaiapp.cn

[Q29] 最大最小值
来源：http://nh.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fr.panjiajie.cn

[Q30] 分组统计
来源：http://ia.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zc.hahajie.cn

[Q31] 分组后过滤
来源：http://du.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://be.9csxet.cn

[Q32] 分组拼接字符串
来源：http://ux.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ea.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ee.wgjwhj.cn

[Q33] 多列分组
来源：http://tm.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ti.521024.cn

[Q34] 每组取第一条
来源：http://hm.yuntaijiaju.cn

SELECT * FROM (
来源：http://oh.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gj.szxytkj.cn

) t WHERE rn = 1;
来源：http://un.shxzukj.cn

[Q35] 内连接
来源：http://yy.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ep.yuntaijiaju.cn

[Q36] 左连接
来源：http://xa.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qx.yuntaijiaju.cn

[Q37] 右连接
来源：http://ib.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ok.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wi.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rj.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://ib.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rz.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hh.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gw.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zt.jctech888.com.cn

[Q41] 多表连接
来源：http://av.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qr.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://jd.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://cq.521024.cn

[Q42] 连接条件附加过滤
来源：http://sh.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://su.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hl.huanxung.cn

[Q43] 标量子查询
来源：http://jk.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zw.gzmigu.cn

[Q44] IN 子查询
来源：http://wh.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mo.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://vh.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://be.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pq.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oi.colortex.cn

[Q47] 与平均值比较
来源：http://xu.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ok.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://sq.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://am.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://nl.wgjwhj.cn

[Q49] 更新单行
来源：http://sm.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xi.gzmigu.cn

[Q50] 批量更新
来源：http://fa.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://at.muxihuayi.cn

[Q51] 用子查询更新
来源：http://gn.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://am.asd995.cn

[Q52] 删除指定行
来源：http://gc.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://of.521024.cn

[Q53] 按条件删除
来源：http://op.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dc.hahajie.cn

[Q54] 清空表
来源：http://pp.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://cn.szsharing.cn

[Q55] 排名（并列占位）
来源：http://ic.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xh.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://hp.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zq.hahajie.cn

[Q57] 行号
来源：http://df.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eb.szsharing.cn

[Q58] 累计求和
来源：http://wh.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://co.shxzskj.cn

[Q59] 分组内累计
来源：http://ad.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bz.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://fa.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zu.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://na.panjiajie.cn

[Q61] 移动平均
来源：http://ty.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cg.huixinmuqiang.cn

[Q62] 分组占比
来源：http://zf.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://za.chemitech.net.cn

[Q63] 开启事务
来源：http://bx.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lt.jianghongdianzi.cn

[Q64] 提交事务
来源：http://ss.nszjky.cn

COMMIT;
来源：http://ar.gzmigu.cn

[Q65] 回滚事务
来源：http://up.shxzskj.cn

ROLLBACK;
来源：http://kx.lnxyls.cn

[Q66] 行锁查询
来源：http://pr.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vf.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://dg.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ri.colortex.cn

[Q68] 保存点
来源：http://nz.szsharing.cn

SAVEPOINT sp1;
来源：http://pl.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://ii.hahajie.cn

[Q69] 查看执行计划
来源：http://yi.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bv.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://pa.yuexingan06.cn

ANALYZE TABLE users;
来源：http://ws.newstarts.cn

[Q71] 查看建表语句
来源：http://ji.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mn.huixinmuqiang.cn

[Q72] 查看索引
来源：http://hf.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://rl.szxytkj.cn

[Q73] 查看表状态
来源：http://qg.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ln.gzmigu.cn

[Q74] 强制使用索引
来源：http://vk.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pt.521024.cn

[Q75] 日期格式化
来源：http://or.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hv.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uy.colortex.cn

[Q76] 按天统计
来源：http://ok.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hk.wgjwhj.cn

[Q77] 时间加减
来源：http://el.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nx.521024.cn

[Q78] 当前时间
来源：http://sl.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://om.shtwfgs.cn

[Q79] 字符串拼接
来源：http://vs.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fy.muxihuayi.cn

[Q80] 字符串截取
来源：http://qj.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rq.shxzskj.cn

[Q81] 字符串替换
来源：http://yo.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pu.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://kb.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xy.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://nk.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cn.521024.cn

[Q84] 去除首尾空格
来源：http://wj.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://nv.521024.cn

[Q85] 数值取整
来源：http://bf.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hv.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://as.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gw.asd995.cn

[Q87] JSON 字段做条件
来源：http://vp.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qs.521024.cn

[Q88] 行转列（条件聚合）
来源：http://mq.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nf.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://os.hahajie.cn

[Q89] 判断表是否存在
来源：http://so.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ex.nicolike.cn

[Q90] 生成序号列
来源：http://ux.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mv.bookmarksfly.cn

================================================================================
来源：http://kp.jctech888.com.cn

R. Bash 专题
来源：http://zv.bookmarksfly.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://jg.521024.cn

#!/usr/bin/env bash
来源：http://yv.jctech888.com.cn

set -euo pipefail
来源：http://wk.9csxet.cn

[R02] 变量赋值与使用
来源：http://ge.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ct.newstarts.cn

[R03] 只读变量
来源：http://od.nszjky.cn


<!-- 参考信息 -->