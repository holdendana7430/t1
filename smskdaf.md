代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://uf.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ck.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://tx.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://dc.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hm.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pf.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://pf.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://az.9csxet.cn

[O06] 使用进程池
来源：http://ii.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zr.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fb.asd995.cn

JS:   // child_process / cluster 模块
来源：http://jh.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://zt.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://je.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yu.jianghongdianzi.cn

Ruby: // fork 块
来源：http://ov.nicolike.cn

C#:   Parallel.For
来源：http://bo.9csxet.cn

================================================================================
来源：http://iz.hnjuh.cn

P. 常用工具函数
来源：http://gi.9csxet.cn

================================================================================
来源：http://vv.521024.cn

[P01] 生成 UUID
来源：http://iw.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://rr.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eq.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://gm.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://um.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://ci.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://au.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://jf.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://ov.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://qs.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://in.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zc.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mu.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tc.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://at.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kb.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://js.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://au.newstarts.cn

[P03] 生成短随机字符串
来源：http://ia.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wz.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://va.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nd.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://px.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hb.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mp.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fp.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wb.huanxung.cn

[P04] 求长度
来源：http://va.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wp.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cp.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yz.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nf.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://tg.asd995.cn

Go:   len(arr);  len(m)
来源：http://ql.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://kn.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ji.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://tg.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bk.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eq.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gk.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sg.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ay.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ri.gzmigu.cn

Ruby: a == b
来源：http://qx.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vs.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oz.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pm.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://pf.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uc.shxzukj.cn

TS:   if (x == null) {}
来源：http://nj.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ok.521024.cn

Go:   if x == nil {}
来源：http://cx.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dr.yuexingan06.cn

C#:   if (x is null) {}
来源：http://pf.szsharing.cn

[P07] 防抖与节流
来源：http://fc.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qw.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://zc.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yt.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cw.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fc.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nu.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aw.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://aj.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pu.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ug.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ah.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lm.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gm.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zc.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fh.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ow.muxihuayi.cn

================================================================================
来源：http://lt.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hf.jctech888.com.cn

================================================================================
来源：http://hw.yuexingan06.cn

[Q01] 创建表
来源：http://hf.wgjwhj.cn

CREATE TABLE users (
来源：http://lz.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nk.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://kj.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://yr.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ma.chemitech.net.cn

);
来源：http://bx.nicolike.cn

[Q02] 创建带外键的表
来源：http://ym.chemitech.net.cn

CREATE TABLE orders (
来源：http://ka.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vz.yuexingan06.cn

user_id INT NOT NULL,
来源：http://hu.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://el.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://le.haigaiapp.cn

);
来源：http://dx.lnxyls.cn

[Q03] 增加列
来源：http://tz.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sg.yuexingan06.cn

[Q04] 修改列类型
来源：http://sw.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yn.wgjwhj.cn

[Q05] 重命名列
来源：http://yg.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vu.jianghongdianzi.cn

[Q06] 删除列
来源：http://ab.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sj.shtwfgs.cn

[Q07] 删除表
来源：http://os.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://kc.hahajie.cn

[Q08] 创建普通索引
来源：http://ux.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ua.shxzukj.cn

[Q09] 创建唯一索引
来源：http://kk.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jx.hahajie.cn

[Q10] 插入单行
来源：http://cb.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oo.shxzskj.cn

[Q11] 一次插入多行
来源：http://wa.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wf.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://yz.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gz.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mn.9csxet.cn

[Q13] 忽略重复插入
来源：http://at.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zm.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://yi.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gr.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wq.huixinmuqiang.cn

[Q15] 查询全部
来源：http://yf.nszjky.cn

SELECT * FROM users;
来源：http://mk.haigaiapp.cn

[Q16] 查询指定列
来源：http://vd.szxytkj.cn

SELECT id, name FROM users;
来源：http://wa.lnxyls.cn

[Q17] 条件查询
来源：http://ez.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fd.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://sk.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jh.bookmarksfly.cn

[Q19] 范围查询
来源：http://za.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://il.lnxyls.cn

[Q20] IN 列表
来源：http://qp.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://py.nicolike.cn

[Q21] 空值判断
来源：http://pe.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hb.hnjuh.cn

[Q22] 排序
来源：http://td.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ki.chemitech.net.cn

[Q23] 分页
来源：http://ir.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tn.hahajie.cn

[Q24] 去重
来源：http://et.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://gc.nicolike.cn

[Q25] 只取前 N 条
来源：http://mj.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wt.huanxung.cn

[Q26] 计数
来源：http://to.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://gw.newstarts.cn

[Q27] 条件计数
来源：http://us.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://td.bjjhwx.cn

[Q28] 求和与平均
来源：http://de.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rq.9csxet.cn

[Q29] 最大最小值
来源：http://kl.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zn.521024.cn

[Q30] 分组统计
来源：http://yd.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dq.hnjuh.cn

[Q31] 分组后过滤
来源：http://ue.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kx.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://ac.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vp.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sb.gzmigu.cn

[Q33] 多列分组
来源：http://xa.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sk.szxytkj.cn

[Q34] 每组取第一条
来源：http://tl.shtwfgs.cn

SELECT * FROM (
来源：http://li.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xh.szxytkj.cn

) t WHERE rn = 1;
来源：http://cf.jctech888.com.cn

[Q35] 内连接
来源：http://al.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wh.lnxyls.cn

[Q36] 左连接
来源：http://ho.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nr.9csxet.cn

[Q37] 右连接
来源：http://vu.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ls.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ex.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bs.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://tn.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yi.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ua.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tj.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nh.shtwfgs.cn

[Q41] 多表连接
来源：http://ob.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zm.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://eb.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://hu.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://gx.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://cu.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vh.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://xm.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oc.yuexingan06.cn

[Q44] IN 子查询
来源：http://yr.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cx.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://km.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ql.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iu.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jy.panjiajie.cn

[Q47] 与平均值比较
来源：http://zi.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bm.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://rz.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://et.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://kv.newstarts.cn

[Q49] 更新单行
来源：http://vc.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vb.hnjuh.cn

[Q50] 批量更新
来源：http://ri.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hy.shxzskj.cn

[Q51] 用子查询更新
来源：http://fa.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yo.hahajie.cn

[Q52] 删除指定行
来源：http://qg.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://wv.colortex.cn

[Q53] 按条件删除
来源：http://bk.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cu.colortex.cn

[Q54] 清空表
来源：http://fb.nszjky.cn

TRUNCATE TABLE logs;
来源：http://na.asd995.cn

[Q55] 排名（并列占位）
来源：http://la.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jw.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://gd.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fz.huixiangedu.cn

[Q57] 行号
来源：http://cl.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gq.colortex.cn

[Q58] 累计求和
来源：http://vj.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ue.shtwfgs.cn

[Q59] 分组内累计
来源：http://vv.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://el.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://jm.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uz.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://je.haigaiapp.cn

[Q61] 移动平均
来源：http://nb.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ji.nszjky.cn

[Q62] 分组占比
来源：http://rm.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gl.panjiajie.cn

[Q63] 开启事务
来源：http://ly.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uu.szxytkj.cn

[Q64] 提交事务
来源：http://ee.hnjuh.cn

COMMIT;
来源：http://da.521024.cn

[Q65] 回滚事务
来源：http://ne.shxzukj.cn

ROLLBACK;
来源：http://fl.bjjhwx.cn

[Q66] 行锁查询
来源：http://sa.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ps.lnxyls.cn

[Q67] 设置隔离级别
来源：http://fc.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pb.huixiangedu.cn

[Q68] 保存点
来源：http://jx.yuexingan06.cn

SAVEPOINT sp1;
来源：http://yy.colortex.cn

ROLLBACK TO sp1;
来源：http://kd.hahajie.cn

[Q69] 查看执行计划
来源：http://up.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fx.9csxet.cn

[Q70] 更新统计信息
来源：http://cd.szxytkj.cn

ANALYZE TABLE users;
来源：http://lu.asd995.cn

[Q71] 查看建表语句
来源：http://qi.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iu.nszjky.cn

[Q72] 查看索引
来源：http://vp.huanxung.cn

SHOW INDEX FROM users;
来源：http://yh.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://qn.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ib.hahajie.cn

[Q74] 强制使用索引
来源：http://or.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ba.wgjwhj.cn

[Q75] 日期格式化
来源：http://zr.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qm.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hs.haigaiapp.cn

[Q76] 按天统计
来源：http://wc.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bp.wgjwhj.cn

[Q77] 时间加减
来源：http://ba.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bx.shxzskj.cn

[Q78] 当前时间
来源：http://al.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://go.muxihuayi.cn

[Q79] 字符串拼接
来源：http://lb.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://al.bjjhwx.cn

[Q80] 字符串截取
来源：http://ua.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wn.szxytkj.cn

[Q81] 字符串替换
来源：http://ph.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xt.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://lu.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uw.newstarts.cn

[Q83] 大小写转换
来源：http://ja.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gd.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://qo.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://yy.panjiajie.cn

[Q85] 数值取整
来源：http://if.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fk.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://jr.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pb.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://ip.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mu.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://rr.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qx.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://on.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://jh.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://id.asd995.cn

[Q90] 生成序号列
来源：http://ks.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gr.gzmigu.cn

================================================================================
来源：http://fw.hnjuh.cn


<!-- 参考信息 -->