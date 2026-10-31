代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zr.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vf.hahajie.cn

Ruby: threads.map(&:join)
来源：http://zp.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pv.asd995.cn

[O06] 使用进程池
来源：http://cz.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fv.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zg.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://xq.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://oi.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zr.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mb.chemitech.net.cn

Ruby: // fork 块
来源：http://yj.yuntaijiaju.cn

C#:   Parallel.For
来源：http://ab.hnjuh.cn

================================================================================
来源：http://za.wgjwhj.cn

P. 常用工具函数
来源：http://bd.muxihuayi.cn

================================================================================
来源：http://kw.chemitech.net.cn

[P01] 生成 UUID
来源：http://nb.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://hl.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ph.521024.cn

JS:   crypto.randomUUID()
来源：http://jd.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://rd.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://pc.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://he.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://sa.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://ez.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://is.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://am.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ij.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qs.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://es.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yz.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zy.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pt.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mk.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://kh.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bs.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nb.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bx.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://af.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qk.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pb.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bb.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zy.jianghongdianzi.cn

[P04] 求长度
来源：http://pk.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ez.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zo.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dz.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iy.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://wm.szsharing.cn

Go:   len(arr);  len(m)
来源：http://cl.newstarts.cn

Ruby: x.length;  x.size
来源：http://kg.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mr.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://fh.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xs.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vx.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jv.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ez.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ms.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mv.shxzskj.cn

Ruby: a == b
来源：http://ga.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://il.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ii.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ix.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://mh.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ct.szxytkj.cn

TS:   if (x == null) {}
来源：http://pt.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sh.nszjky.cn

Go:   if x == nil {}
来源：http://wz.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://de.521024.cn

C#:   if (x is null) {}
来源：http://ia.panjiajie.cn

[P07] 防抖与节流
来源：http://gr.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dr.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://ie.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iu.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sg.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://om.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bu.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qt.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ob.hahajie.cn

[P08] 处理浮点精度问题
来源：http://ky.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bg.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tv.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gv.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xk.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bl.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sq.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yz.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://an.chemitech.net.cn

================================================================================
来源：http://xv.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kq.yuexingan06.cn

================================================================================
来源：http://lg.muxihuayi.cn

[Q01] 创建表
来源：http://yr.huixiangedu.cn

CREATE TABLE users (
来源：http://kn.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kx.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://wz.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://zj.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bf.chemitech.net.cn

);
来源：http://qh.gzmigu.cn

[Q02] 创建带外键的表
来源：http://la.muxihuayi.cn

CREATE TABLE orders (
来源：http://bv.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xs.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://wx.colortex.cn

amount DECIMAL(10, 2),
来源：http://st.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pj.chemitech.net.cn

);
来源：http://xn.huanxung.cn

[Q03] 增加列
来源：http://kt.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bm.panjiajie.cn

[Q04] 修改列类型
来源：http://dj.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ef.muxihuayi.cn

[Q05] 重命名列
来源：http://ao.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dk.hnjuh.cn

[Q06] 删除列
来源：http://xm.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mq.szsharing.cn

[Q07] 删除表
来源：http://ir.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://qe.szsharing.cn

[Q08] 创建普通索引
来源：http://jf.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vk.gzmigu.cn

[Q09] 创建唯一索引
来源：http://ev.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ka.wgjwhj.cn

[Q10] 插入单行
来源：http://za.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qu.wgjwhj.cn

[Q11] 一次插入多行
来源：http://tr.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nn.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://te.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bh.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rq.asd995.cn

[Q13] 忽略重复插入
来源：http://id.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rg.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://df.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lf.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cr.shxzskj.cn

[Q15] 查询全部
来源：http://pc.9csxet.cn

SELECT * FROM users;
来源：http://qd.shtwfgs.cn

[Q16] 查询指定列
来源：http://zj.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://wi.nszjky.cn

[Q17] 条件查询
来源：http://gc.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rh.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://ft.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qt.colortex.cn

[Q19] 范围查询
来源：http://ll.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hg.shtwfgs.cn

[Q20] IN 列表
来源：http://mu.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://er.shxzukj.cn

[Q21] 空值判断
来源：http://fb.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ca.asd995.cn

[Q22] 排序
来源：http://jt.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yp.nicolike.cn

[Q23] 分页
来源：http://ts.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ms.shxzukj.cn

[Q24] 去重
来源：http://kb.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://th.szxytkj.cn

[Q25] 只取前 N 条
来源：http://hz.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bk.newstarts.cn

[Q26] 计数
来源：http://hw.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://qz.yuexingan06.cn

[Q27] 条件计数
来源：http://sx.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bu.huixiangedu.cn

[Q28] 求和与平均
来源：http://qr.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ti.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://cc.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sh.yuexingan06.cn

[Q30] 分组统计
来源：http://wt.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xy.bjjhwx.cn

[Q31] 分组后过滤
来源：http://uz.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oo.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://ma.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cg.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sj.panjiajie.cn

[Q33] 多列分组
来源：http://iv.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://li.nszjky.cn

[Q34] 每组取第一条
来源：http://sp.haigaiapp.cn

SELECT * FROM (
来源：http://qj.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://di.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://qi.haigaiapp.cn

[Q35] 内连接
来源：http://kn.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hv.newstarts.cn

[Q36] 左连接
来源：http://vp.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vr.newstarts.cn

[Q37] 右连接
来源：http://fb.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eb.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cz.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jk.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://mi.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yk.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dh.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vv.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ju.colortex.cn

[Q41] 多表连接
来源：http://rc.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dr.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://lv.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://hn.colortex.cn

[Q42] 连接条件附加过滤
来源：http://co.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://rl.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jf.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://bo.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xf.szxytkj.cn

[Q44] IN 子查询
来源：http://yk.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rx.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://sw.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oj.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qx.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sf.lnxyls.cn

[Q47] 与平均值比较
来源：http://ru.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yq.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://ft.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ts.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://dp.9csxet.cn

[Q49] 更新单行
来源：http://ad.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xi.chemitech.net.cn

[Q50] 批量更新
来源：http://tl.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yc.shxzskj.cn

[Q51] 用子查询更新
来源：http://mb.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ua.huixiangedu.cn

[Q52] 删除指定行
来源：http://jh.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://pu.jctech888.com.cn

[Q53] 按条件删除
来源：http://mu.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lo.chemitech.net.cn

[Q54] 清空表
来源：http://tr.9csxet.cn

TRUNCATE TABLE logs;
来源：http://me.szsharing.cn

[Q55] 排名（并列占位）
来源：http://xq.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hm.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://zh.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ba.szsharing.cn

[Q57] 行号
来源：http://ow.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://id.lnxyls.cn

[Q58] 累计求和
来源：http://xp.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cp.huanxung.cn

[Q59] 分组内累计
来源：http://rz.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ew.521024.cn

[Q60] 取上一行 / 下一行
来源：http://gs.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wm.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yv.shtwfgs.cn

[Q61] 移动平均
来源：http://yc.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qc.szxytkj.cn

[Q62] 分组占比
来源：http://if.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kt.nszjky.cn

[Q63] 开启事务
来源：http://zr.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ol.yuexingan06.cn

[Q64] 提交事务
来源：http://qa.huixiangedu.cn

COMMIT;
来源：http://pb.chemitech.net.cn

[Q65] 回滚事务
来源：http://gk.jianghongdianzi.cn

ROLLBACK;
来源：http://iz.panjiajie.cn

[Q66] 行锁查询
来源：http://hq.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tz.nszjky.cn

[Q67] 设置隔离级别
来源：http://cz.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dh.nszjky.cn

[Q68] 保存点
来源：http://sm.hahajie.cn

SAVEPOINT sp1;
来源：http://qh.lnxyls.cn

ROLLBACK TO sp1;
来源：http://oq.huanxung.cn

[Q69] 查看执行计划
来源：http://by.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pu.lnxyls.cn

[Q70] 更新统计信息
来源：http://kp.asd995.cn

ANALYZE TABLE users;
来源：http://wz.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://fi.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ts.wgjwhj.cn

[Q72] 查看索引
来源：http://xk.hahajie.cn

SHOW INDEX FROM users;
来源：http://sa.colortex.cn

[Q73] 查看表状态
来源：http://xd.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xw.gzmigu.cn

[Q74] 强制使用索引
来源：http://ip.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qm.nicolike.cn

[Q75] 日期格式化
来源：http://lm.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yd.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ii.colortex.cn

[Q76] 按天统计
来源：http://zw.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lz.wgjwhj.cn

[Q77] 时间加减
来源：http://tc.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ct.muxihuayi.cn

[Q78] 当前时间
来源：http://pd.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ks.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://ql.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pt.bookmarksfly.cn

[Q80] 字符串截取
来源：http://vi.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nd.newstarts.cn

[Q81] 字符串替换
来源：http://id.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ll.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://zz.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lf.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://at.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pa.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://gd.521024.cn

SELECT TRIM(name) FROM users;
来源：http://rk.nszjky.cn

[Q85] 数值取整
来源：http://sc.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uv.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://yz.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fa.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://th.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://na.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://sb.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://do.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jm.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://cr.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://si.jctech888.com.cn

[Q90] 生成序号列
来源：http://bd.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gz.jianghongdianzi.cn

================================================================================
来源：http://qy.wgjwhj.cn

R. Bash 专题
来源：http://zp.wgjwhj.cn

================================================================================
来源：http://hy.shxzukj.cn

[R01] shebang 与严格模式
来源：http://wq.chemitech.net.cn

#!/usr/bin/env bash
来源：http://ae.chemitech.net.cn


<!-- 参考信息 -->