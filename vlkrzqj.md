代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://if.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wv.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://tl.colortex.cn

TS:   await Promise.all(tasks)
来源：http://wj.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jj.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kn.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://ay.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cr.panjiajie.cn

[O06] 使用进程池
来源：http://so.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vv.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ex.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://wj.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://sp.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ex.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yx.huixinmuqiang.cn

Ruby: // fork 块
来源：http://yk.lnxyls.cn

C#:   Parallel.For
来源：http://wn.bookmarksfly.cn

================================================================================
来源：http://jk.shxzukj.cn

P. 常用工具函数
来源：http://hs.panjiajie.cn

================================================================================
来源：http://vd.newstarts.cn

[P01] 生成 UUID
来源：http://vz.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://vd.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oa.newstarts.cn

JS:   crypto.randomUUID()
来源：http://oo.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://vt.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://fq.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://zz.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://iv.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://mh.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://uh.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jc.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ls.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vt.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hf.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yx.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ld.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wi.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fv.asd995.cn

[P03] 生成短随机字符串
来源：http://cw.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nk.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lq.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://io.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gg.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vq.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pr.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ke.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ea.jctech888.com.cn

[P04] 求长度
来源：http://ce.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cs.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tt.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sh.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ny.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://vs.nszjky.cn

Go:   len(arr);  len(m)
来源：http://ew.asd995.cn

Ruby: x.length;  x.size
来源：http://rl.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cz.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://po.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://os.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zv.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eu.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gb.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sm.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dg.huixinmuqiang.cn

Ruby: a == b
来源：http://wu.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mv.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wz.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vw.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://hs.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://as.jctech888.com.cn

TS:   if (x == null) {}
来源：http://ug.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hh.yuexingan06.cn

Go:   if x == nil {}
来源：http://wz.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tk.shxzukj.cn

C#:   if (x is null) {}
来源：http://sm.wgjwhj.cn

[P07] 防抖与节流
来源：http://jl.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dr.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://fj.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aq.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://np.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aq.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zp.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hx.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tz.nszjky.cn

[P08] 处理浮点精度问题
来源：http://hx.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ke.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qo.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qp.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qd.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ep.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mj.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zx.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xp.shxzskj.cn

================================================================================
来源：http://st.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ik.bjjhwx.cn

================================================================================
来源：http://ns.wgjwhj.cn

[Q01] 创建表
来源：http://pf.521024.cn

CREATE TABLE users (
来源：http://li.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fl.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://oi.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ji.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kl.huixiangedu.cn

);
来源：http://ra.newstarts.cn

[Q02] 创建带外键的表
来源：http://fd.haigaiapp.cn

CREATE TABLE orders (
来源：http://yu.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rp.asd995.cn

user_id INT NOT NULL,
来源：http://cu.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://yy.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hl.huixinmuqiang.cn

);
来源：http://hj.haigaiapp.cn

[Q03] 增加列
来源：http://ug.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qi.newstarts.cn

[Q04] 修改列类型
来源：http://ji.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nh.hahajie.cn

[Q05] 重命名列
来源：http://xj.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ju.huixinmuqiang.cn

[Q06] 删除列
来源：http://ty.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pv.shxzukj.cn

[Q07] 删除表
来源：http://df.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://ra.gzmigu.cn

[Q08] 创建普通索引
来源：http://oi.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oq.szsharing.cn

[Q09] 创建唯一索引
来源：http://kl.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wc.hnjuh.cn

[Q10] 插入单行
来源：http://cl.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ii.newstarts.cn

[Q11] 一次插入多行
来源：http://rk.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://os.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://nd.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tt.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mc.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://cm.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zx.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://zm.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ua.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ap.9csxet.cn

[Q15] 查询全部
来源：http://km.panjiajie.cn

SELECT * FROM users;
来源：http://nz.asd995.cn

[Q16] 查询指定列
来源：http://qy.szsharing.cn

SELECT id, name FROM users;
来源：http://qx.wgjwhj.cn

[Q17] 条件查询
来源：http://qu.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pi.521024.cn

[Q18] 模糊匹配
来源：http://go.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mi.jianghongdianzi.cn

[Q19] 范围查询
来源：http://nv.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wh.colortex.cn

[Q20] IN 列表
来源：http://xd.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fn.gzmigu.cn

[Q21] 空值判断
来源：http://fk.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ki.asd995.cn

[Q22] 排序
来源：http://ix.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sv.yuexingan06.cn

[Q23] 分页
来源：http://bl.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fp.yuexingan06.cn

[Q24] 去重
来源：http://bh.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://kh.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://vh.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rd.muxihuayi.cn

[Q26] 计数
来源：http://nf.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://pa.bjjhwx.cn

[Q27] 条件计数
来源：http://sc.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dw.colortex.cn

[Q28] 求和与平均
来源：http://od.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zu.shxzukj.cn

[Q29] 最大最小值
来源：http://dg.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://an.nicolike.cn

[Q30] 分组统计
来源：http://fp.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ul.huanxung.cn

[Q31] 分组后过滤
来源：http://qa.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://si.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://su.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cj.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ot.gzmigu.cn

[Q33] 多列分组
来源：http://lj.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mr.gzmigu.cn

[Q34] 每组取第一条
来源：http://jf.nszjky.cn

SELECT * FROM (
来源：http://zv.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fa.asd995.cn

) t WHERE rn = 1;
来源：http://eo.szxytkj.cn

[Q35] 内连接
来源：http://lr.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ok.9csxet.cn

[Q36] 左连接
来源：http://cn.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lg.chemitech.net.cn

[Q37] 右连接
来源：http://ol.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ne.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jb.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oa.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://qw.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ia.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pm.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vq.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nf.jianghongdianzi.cn

[Q41] 多表连接
来源：http://kp.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tm.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://dn.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://ap.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://os.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://xq.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nz.szxytkj.cn

[Q43] 标量子查询
来源：http://lu.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tp.wgjwhj.cn

[Q44] IN 子查询
来源：http://vs.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zq.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://xi.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bw.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://di.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://om.gzmigu.cn

[Q47] 与平均值比较
来源：http://eu.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ig.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://wl.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pm.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ms.jctech888.com.cn

[Q49] 更新单行
来源：http://ur.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dw.yuexingan06.cn

[Q50] 批量更新
来源：http://sj.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xp.chemitech.net.cn

[Q51] 用子查询更新
来源：http://ui.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://or.nicolike.cn

[Q52] 删除指定行
来源：http://ig.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://dz.asd995.cn

[Q53] 按条件删除
来源：http://ul.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mf.hahajie.cn

[Q54] 清空表
来源：http://zm.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://uz.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://wn.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ig.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://je.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dk.asd995.cn

[Q57] 行号
来源：http://ox.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rz.wgjwhj.cn

[Q58] 累计求和
来源：http://qw.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wz.nicolike.cn

[Q59] 分组内累计
来源：http://zf.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ne.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://ie.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ob.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lq.nicolike.cn

[Q61] 移动平均
来源：http://pt.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://np.muxihuayi.cn

[Q62] 分组占比
来源：http://dz.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ar.muxihuayi.cn

[Q63] 开启事务
来源：http://vw.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gz.newstarts.cn

[Q64] 提交事务
来源：http://ca.521024.cn

COMMIT;
来源：http://ia.newstarts.cn

[Q65] 回滚事务
来源：http://ye.gzmigu.cn

ROLLBACK;
来源：http://fd.jctech888.com.cn

[Q66] 行锁查询
来源：http://fd.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pq.panjiajie.cn

[Q67] 设置隔离级别
来源：http://ar.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wj.yuexingan06.cn

[Q68] 保存点
来源：http://fh.asd995.cn

SAVEPOINT sp1;
来源：http://tj.shxzukj.cn

ROLLBACK TO sp1;
来源：http://kp.hahajie.cn

[Q69] 查看执行计划
来源：http://tb.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qi.asd995.cn

[Q70] 更新统计信息
来源：http://fi.newstarts.cn

ANALYZE TABLE users;
来源：http://tv.521024.cn

[Q71] 查看建表语句
来源：http://hn.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gk.asd995.cn

[Q72] 查看索引
来源：http://aq.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://el.gzmigu.cn

[Q73] 查看表状态
来源：http://he.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jy.hahajie.cn

[Q74] 强制使用索引
来源：http://qp.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rr.521024.cn

[Q75] 日期格式化
来源：http://nw.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gl.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pu.muxihuayi.cn

[Q76] 按天统计
来源：http://ja.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://un.lnxyls.cn

[Q77] 时间加减
来源：http://ao.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ea.huanxung.cn

[Q78] 当前时间
来源：http://jr.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ib.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://zk.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xd.9csxet.cn

[Q80] 字符串截取
来源：http://wg.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fe.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://uy.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xf.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://bg.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mc.yuexingan06.cn

[Q83] 大小写转换
来源：http://zp.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mg.gzmigu.cn

[Q84] 去除首尾空格
来源：http://sb.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://tc.yuntaijiaju.cn

[Q85] 数值取整
来源：http://je.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ju.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://aq.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cn.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://jg.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lh.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://kn.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gu.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://za.gzmigu.cn

[Q89] 判断表是否存在
来源：http://bu.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mh.huanxung.cn

[Q90] 生成序号列
来源：http://kc.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hi.shxzskj.cn

================================================================================
来源：http://vd.bjjhwx.cn


<!-- 参考信息 -->