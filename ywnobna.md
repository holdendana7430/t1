代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://yq.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xv.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://mj.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://yw.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ef.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ad.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://qq.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://so.nszjky.cn

[O06] 使用进程池
来源：http://kg.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xu.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xy.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://ww.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://rm.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oa.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gr.hnjuh.cn

Ruby: // fork 块
来源：http://gl.wgjwhj.cn

C#:   Parallel.For
来源：http://lb.yuexingan06.cn

================================================================================
来源：http://fj.hahajie.cn

P. 常用工具函数
来源：http://gi.bookmarksfly.cn

================================================================================
来源：http://be.wgjwhj.cn

[P01] 生成 UUID
来源：http://mp.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://bf.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vy.huanxung.cn

JS:   crypto.randomUUID()
来源：http://bj.hahajie.cn

TS:   crypto.randomUUID()
来源：http://er.521024.cn

Java: UUID.randomUUID().toString()
来源：http://hx.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://ve.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://sr.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://js.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://pi.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qu.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pf.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pe.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tr.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kg.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lj.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sy.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dq.shxzukj.cn

[P03] 生成短随机字符串
来源：http://hm.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ay.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lq.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pq.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mb.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fs.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ip.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ar.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ts.yuexingan06.cn

[P04] 求长度
来源：http://xe.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://je.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pm.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mj.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xy.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://ty.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://lx.9csxet.cn

Ruby: x.length;  x.size
来源：http://nn.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kv.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://jq.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ky.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pm.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pc.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jr.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jm.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nr.nicolike.cn

Ruby: a == b
来源：http://nx.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hi.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lg.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fp.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://pg.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lz.lnxyls.cn

TS:   if (x == null) {}
来源：http://ws.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xa.asd995.cn

Go:   if x == nil {}
来源：http://po.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vw.nicolike.cn

C#:   if (x is null) {}
来源：http://de.haigaiapp.cn

[P07] 防抖与节流
来源：http://nb.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://py.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://tl.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zm.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ch.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vr.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://go.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iy.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lj.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ox.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kt.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://an.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tj.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ph.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fg.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lh.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dh.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dy.huixiangedu.cn

================================================================================
来源：http://az.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ne.huixinmuqiang.cn

================================================================================
来源：http://fk.panjiajie.cn

[Q01] 创建表
来源：http://vw.hahajie.cn

CREATE TABLE users (
来源：http://vr.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xw.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://fk.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://fj.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vz.jianghongdianzi.cn

);
来源：http://ww.hahajie.cn

[Q02] 创建带外键的表
来源：http://yp.colortex.cn

CREATE TABLE orders (
来源：http://yb.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dg.huixiangedu.cn

user_id INT NOT NULL,
来源：http://zb.szsharing.cn

amount DECIMAL(10, 2),
来源：http://zm.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ao.asd995.cn

);
来源：http://xk.jctech888.com.cn

[Q03] 增加列
来源：http://nf.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ur.shxzukj.cn

[Q04] 修改列类型
来源：http://xh.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xg.asd995.cn

[Q05] 重命名列
来源：http://kv.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cw.jianghongdianzi.cn

[Q06] 删除列
来源：http://gt.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pf.haigaiapp.cn

[Q07] 删除表
来源：http://wf.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://gm.colortex.cn

[Q08] 创建普通索引
来源：http://fg.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tm.hahajie.cn

[Q09] 创建唯一索引
来源：http://ii.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yf.lnxyls.cn

[Q10] 插入单行
来源：http://bh.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gd.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://bi.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lu.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://wl.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zq.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fk.lnxyls.cn

[Q13] 忽略重复插入
来源：http://lx.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ww.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://gb.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ww.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://by.colortex.cn

[Q15] 查询全部
来源：http://ou.newstarts.cn

SELECT * FROM users;
来源：http://iz.shxzskj.cn

[Q16] 查询指定列
来源：http://yp.521024.cn

SELECT id, name FROM users;
来源：http://jx.muxihuayi.cn

[Q17] 条件查询
来源：http://sb.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wq.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://jm.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lx.szxytkj.cn

[Q19] 范围查询
来源：http://na.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cq.wgjwhj.cn

[Q20] IN 列表
来源：http://de.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dy.yuntaijiaju.cn

[Q21] 空值判断
来源：http://sb.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://el.jctech888.com.cn

[Q22] 排序
来源：http://nq.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gp.hahajie.cn

[Q23] 分页
来源：http://jy.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://te.muxihuayi.cn

[Q24] 去重
来源：http://ci.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://wz.newstarts.cn

[Q25] 只取前 N 条
来源：http://qz.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hr.hnjuh.cn

[Q26] 计数
来源：http://ll.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ry.9csxet.cn

[Q27] 条件计数
来源：http://jl.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ek.asd995.cn

[Q28] 求和与平均
来源：http://up.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ta.huixiangedu.cn

[Q29] 最大最小值
来源：http://iy.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qh.jianghongdianzi.cn

[Q30] 分组统计
来源：http://vq.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nq.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://le.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mw.hahajie.cn

[Q32] 分组拼接字符串
来源：http://yj.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pz.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://be.lnxyls.cn

[Q33] 多列分组
来源：http://wv.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wp.szxytkj.cn

[Q34] 每组取第一条
来源：http://zg.gzmigu.cn

SELECT * FROM (
来源：http://py.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jw.chemitech.net.cn

) t WHERE rn = 1;
来源：http://aw.jianghongdianzi.cn

[Q35] 内连接
来源：http://sb.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qh.huixiangedu.cn

[Q36] 左连接
来源：http://aw.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ef.nszjky.cn

[Q37] 右连接
来源：http://yy.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gd.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tu.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pn.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://zr.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fo.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vi.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zr.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jm.wgjwhj.cn

[Q41] 多表连接
来源：http://rs.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://as.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://mj.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://zn.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://ef.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://ez.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://al.wgjwhj.cn

[Q43] 标量子查询
来源：http://cf.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://by.newstarts.cn

[Q44] IN 子查询
来源：http://qo.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yn.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://bn.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bg.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vv.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zn.wgjwhj.cn

[Q47] 与平均值比较
来源：http://jd.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fd.asd995.cn

[Q48] CTE 公用表表达式
来源：http://bn.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://it.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://qt.nicolike.cn

[Q49] 更新单行
来源：http://kk.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nd.jctech888.com.cn

[Q50] 批量更新
来源：http://jv.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ve.wgjwhj.cn

[Q51] 用子查询更新
来源：http://rf.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bz.gzmigu.cn

[Q52] 删除指定行
来源：http://up.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://lr.bookmarksfly.cn

[Q53] 按条件删除
来源：http://nz.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ai.nszjky.cn

[Q54] 清空表
来源：http://fr.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://qb.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://tk.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ak.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://yw.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fk.hnjuh.cn

[Q57] 行号
来源：http://qn.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lr.asd995.cn

[Q58] 累计求和
来源：http://jd.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jp.hahajie.cn

[Q59] 分组内累计
来源：http://xg.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jp.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://on.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sv.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nz.hnjuh.cn

[Q61] 移动平均
来源：http://bq.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ki.nszjky.cn

[Q62] 分组占比
来源：http://kd.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zw.nicolike.cn

[Q63] 开启事务
来源：http://lv.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rj.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ok.huanxung.cn

COMMIT;
来源：http://rf.colortex.cn

[Q65] 回滚事务
来源：http://nr.521024.cn

ROLLBACK;
来源：http://ya.huanxung.cn

[Q66] 行锁查询
来源：http://vc.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://za.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://mv.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ip.huanxung.cn

[Q68] 保存点
来源：http://zm.gzmigu.cn

SAVEPOINT sp1;
来源：http://pc.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://jo.newstarts.cn

[Q69] 查看执行计划
来源：http://hh.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xt.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://iu.nszjky.cn

ANALYZE TABLE users;
来源：http://dk.huanxung.cn

[Q71] 查看建表语句
来源：http://ae.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yr.bjjhwx.cn

[Q72] 查看索引
来源：http://pc.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://sy.muxihuayi.cn

[Q73] 查看表状态
来源：http://lh.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xg.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://pq.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gt.colortex.cn

[Q75] 日期格式化
来源：http://um.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gh.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ms.wgjwhj.cn

[Q76] 按天统计
来源：http://hz.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uj.asd995.cn

[Q77] 时间加减
来源：http://pd.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mw.huanxung.cn

[Q78] 当前时间
来源：http://jr.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ml.gzmigu.cn

[Q79] 字符串拼接
来源：http://eq.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cm.gzmigu.cn

[Q80] 字符串截取
来源：http://zx.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dw.yuexingan06.cn

[Q81] 字符串替换
来源：http://sd.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qo.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://gx.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://em.yuexingan06.cn

[Q83] 大小写转换
来源：http://si.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rq.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://da.521024.cn

SELECT TRIM(name) FROM users;
来源：http://cs.hahajie.cn

[Q85] 数值取整
来源：http://zp.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dx.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://rq.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rl.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://fg.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rh.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://oy.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nv.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kg.szsharing.cn

[Q89] 判断表是否存在
来源：http://pc.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oz.lnxyls.cn

[Q90] 生成序号列
来源：http://lw.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://km.haigaiapp.cn

================================================================================
来源：http://jn.yuexingan06.cn


<!-- 参考信息 -->