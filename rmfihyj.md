代发 wailian999

[O06] 使用进程池
来源：http://kv.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ej.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://az.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://mv.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://cw.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qq.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jf.shxzskj.cn

Ruby: // fork 块
来源：http://in.nszjky.cn

C#:   Parallel.For
来源：http://ev.colortex.cn

================================================================================
来源：http://fk.szxytkj.cn

P. 常用工具函数
来源：http://cu.huixiangedu.cn

================================================================================
来源：http://en.chemitech.net.cn

[P01] 生成 UUID
来源：http://yo.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://vm.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ij.szsharing.cn

JS:   crypto.randomUUID()
来源：http://yl.newstarts.cn

TS:   crypto.randomUUID()
来源：http://xd.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://xz.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://eo.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://eo.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://cd.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://it.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xl.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tg.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gd.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dg.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ew.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lb.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gk.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ob.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://ic.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tu.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hr.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ho.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fl.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lp.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jx.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ds.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ns.huixiangedu.cn

[P04] 求长度
来源：http://th.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yf.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pn.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vh.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ls.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://mb.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://wy.colortex.cn

Ruby: x.length;  x.size
来源：http://sl.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hr.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://uo.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dq.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hj.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yl.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ph.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ou.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ph.gzmigu.cn

Ruby: a == b
来源：http://in.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xr.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bk.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pa.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://yx.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ru.nszjky.cn

TS:   if (x == null) {}
来源：http://rq.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zj.bookmarksfly.cn

Go:   if x == nil {}
来源：http://yi.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uv.wgjwhj.cn

C#:   if (x is null) {}
来源：http://od.szsharing.cn

[P07] 防抖与节流
来源：http://op.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gv.521024.cn

PHP:  // 手写时间戳比较
来源：http://wm.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://il.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yr.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lb.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kn.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yo.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uj.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://my.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://st.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wb.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ho.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rv.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qt.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xf.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qc.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vh.hnjuh.cn

================================================================================
来源：http://xe.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pi.shxzukj.cn

================================================================================
来源：http://su.panjiajie.cn

[Q01] 创建表
来源：http://tr.hahajie.cn

CREATE TABLE users (
来源：http://pf.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://on.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://uk.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://st.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nw.huixinmuqiang.cn

);
来源：http://pb.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://tf.szxytkj.cn

CREATE TABLE orders (
来源：http://vm.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ps.shxzukj.cn

user_id INT NOT NULL,
来源：http://wa.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://pw.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rx.newstarts.cn

);
来源：http://mc.haigaiapp.cn

[Q03] 增加列
来源：http://mg.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dy.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://aw.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ac.bjjhwx.cn

[Q05] 重命名列
来源：http://ah.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vz.nicolike.cn

[Q06] 删除列
来源：http://wz.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jz.yuexingan06.cn

[Q07] 删除表
来源：http://qz.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ky.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://zj.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bp.huanxung.cn

[Q09] 创建唯一索引
来源：http://za.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zb.jianghongdianzi.cn

[Q10] 插入单行
来源：http://ok.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ma.asd995.cn

[Q11] 一次插入多行
来源：http://ub.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nq.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://lb.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sn.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ll.shxzukj.cn

[Q13] 忽略重复插入
来源：http://uc.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ns.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://oi.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pa.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ds.colortex.cn

[Q15] 查询全部
来源：http://rw.hnjuh.cn

SELECT * FROM users;
来源：http://cw.colortex.cn

[Q16] 查询指定列
来源：http://eb.asd995.cn

SELECT id, name FROM users;
来源：http://oa.huixinmuqiang.cn

[Q17] 条件查询
来源：http://ms.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uz.huanxung.cn

[Q18] 模糊匹配
来源：http://cp.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tp.haigaiapp.cn

[Q19] 范围查询
来源：http://wp.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rz.colortex.cn

[Q20] IN 列表
来源：http://np.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nb.colortex.cn

[Q21] 空值判断
来源：http://uz.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wx.bookmarksfly.cn

[Q22] 排序
来源：http://au.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vk.szxytkj.cn

[Q23] 分页
来源：http://yh.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qs.jianghongdianzi.cn

[Q24] 去重
来源：http://tx.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://ku.colortex.cn

[Q25] 只取前 N 条
来源：http://qx.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kd.huixiangedu.cn

[Q26] 计数
来源：http://qm.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://cj.gzmigu.cn

[Q27] 条件计数
来源：http://bq.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ln.huixiangedu.cn

[Q28] 求和与平均
来源：http://dv.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yh.asd995.cn

[Q29] 最大最小值
来源：http://br.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://if.haigaiapp.cn

[Q30] 分组统计
来源：http://vz.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yj.haigaiapp.cn

[Q31] 分组后过滤
来源：http://dz.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iz.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://sx.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rq.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cc.nicolike.cn

[Q33] 多列分组
来源：http://ea.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rc.asd995.cn

[Q34] 每组取第一条
来源：http://kf.hnjuh.cn

SELECT * FROM (
来源：http://sm.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fd.hahajie.cn

) t WHERE rn = 1;
来源：http://ps.colortex.cn

[Q35] 内连接
来源：http://ee.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lv.wgjwhj.cn

[Q36] 左连接
来源：http://zs.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xg.yuntaijiaju.cn

[Q37] 右连接
来源：http://qp.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dt.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qy.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mt.asd995.cn

[Q39] 自连接（查上下级）
来源：http://uw.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dx.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ch.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tv.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://be.hahajie.cn

[Q41] 多表连接
来源：http://cj.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dx.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://xr.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://li.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://yr.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://cd.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sy.nszjky.cn

[Q43] 标量子查询
来源：http://iy.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ns.hnjuh.cn

[Q44] IN 子查询
来源：http://al.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ut.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://yo.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hx.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xi.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ky.shtwfgs.cn

[Q47] 与平均值比较
来源：http://uk.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jq.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://ps.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rw.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://oe.gzmigu.cn

[Q49] 更新单行
来源：http://gf.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gi.lnxyls.cn

[Q50] 批量更新
来源：http://gt.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ty.yuexingan06.cn

[Q51] 用子查询更新
来源：http://bh.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hf.chemitech.net.cn

[Q52] 删除指定行
来源：http://wx.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://gi.szxytkj.cn

[Q53] 按条件删除
来源：http://il.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tz.hahajie.cn

[Q54] 清空表
来源：http://yr.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://qb.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://jd.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ki.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://wy.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pc.haigaiapp.cn

[Q57] 行号
来源：http://xm.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dc.yuexingan06.cn

[Q58] 累计求和
来源：http://jo.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dz.huanxung.cn

[Q59] 分组内累计
来源：http://ol.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gy.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://qu.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ty.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ej.lnxyls.cn

[Q61] 移动平均
来源：http://rz.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xw.asd995.cn

[Q62] 分组占比
来源：http://gz.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sz.asd995.cn

[Q63] 开启事务
来源：http://yu.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vt.gzmigu.cn

[Q64] 提交事务
来源：http://nn.wgjwhj.cn

COMMIT;
来源：http://vn.newstarts.cn

[Q65] 回滚事务
来源：http://bo.muxihuayi.cn

ROLLBACK;
来源：http://wj.wgjwhj.cn

[Q66] 行锁查询
来源：http://uq.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mv.huanxung.cn

[Q67] 设置隔离级别
来源：http://nb.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://to.bookmarksfly.cn

[Q68] 保存点
来源：http://od.haigaiapp.cn

SAVEPOINT sp1;
来源：http://nq.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://tc.gzmigu.cn

[Q69] 查看执行计划
来源：http://us.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fh.newstarts.cn

[Q70] 更新统计信息
来源：http://bb.hnjuh.cn

ANALYZE TABLE users;
来源：http://zd.szsharing.cn

[Q71] 查看建表语句
来源：http://rt.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zo.huixiangedu.cn

[Q72] 查看索引
来源：http://dp.shxzukj.cn

SHOW INDEX FROM users;
来源：http://ph.gzmigu.cn

[Q73] 查看表状态
来源：http://td.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dn.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ot.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ma.jctech888.com.cn

[Q75] 日期格式化
来源：http://tt.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dg.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lu.huixinmuqiang.cn

[Q76] 按天统计
来源：http://cp.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pc.panjiajie.cn

[Q77] 时间加减
来源：http://gj.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tu.9csxet.cn

[Q78] 当前时间
来源：http://pz.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pb.bjjhwx.cn

[Q79] 字符串拼接
来源：http://zo.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jo.szsharing.cn

[Q80] 字符串截取
来源：http://bk.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pv.lnxyls.cn

[Q81] 字符串替换
来源：http://fa.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yr.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://at.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pz.muxihuayi.cn

[Q83] 大小写转换
来源：http://vy.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xa.hnjuh.cn

[Q84] 去除首尾空格
来源：http://xv.521024.cn

SELECT TRIM(name) FROM users;
来源：http://kz.jctech888.com.cn

[Q85] 数值取整
来源：http://ud.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qw.asd995.cn

[Q86] 读取 JSON 字段
来源：http://xf.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vd.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://we.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lm.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://ow.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://it.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cl.asd995.cn

[Q89] 判断表是否存在
来源：http://dk.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://du.521024.cn

[Q90] 生成序号列
来源：http://rn.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gd.shtwfgs.cn

================================================================================
来源：http://fw.colortex.cn

R. Bash 专题
来源：http://db.nicolike.cn

================================================================================
来源：http://nn.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://yc.asd995.cn

#!/usr/bin/env bash
来源：http://hl.haigaiapp.cn

set -euo pipefail
来源：http://zm.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://he.panjiajie.cn

name="Tom"; echo "$name"
来源：http://br.huixinmuqiang.cn

[R03] 只读变量
来源：http://hf.nszjky.cn


<!-- 参考信息 -->