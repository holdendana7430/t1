代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://lh.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vo.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://ec.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://go.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uu.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jm.nicolike.cn

Ruby: threads.map(&:join)
来源：http://pg.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://am.yuntaijiaju.cn

[O06] 使用进程池
来源：http://nn.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kp.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xn.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://va.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://ds.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ix.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ul.jianghongdianzi.cn

Ruby: // fork 块
来源：http://ej.newstarts.cn

C#:   Parallel.For
来源：http://kq.colortex.cn

================================================================================
来源：http://xp.bjjhwx.cn

P. 常用工具函数
来源：http://el.szxytkj.cn

================================================================================
来源：http://rm.nicolike.cn

[P01] 生成 UUID
来源：http://gv.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ab.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xc.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://ha.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://zx.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://vg.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://dv.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ev.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://mb.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://kw.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://en.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ki.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bg.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ij.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jq.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://su.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uf.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dx.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://go.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kd.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dr.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aa.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ns.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ny.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bw.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ao.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qi.bjjhwx.cn

[P04] 求长度
来源：http://dz.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gc.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jg.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rs.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zz.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://ii.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://vl.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://nr.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://va.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://xn.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://la.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ce.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gr.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dj.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zy.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yx.shxzukj.cn

Ruby: a == b
来源：http://zy.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jv.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yw.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ri.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://rz.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cl.9csxet.cn

TS:   if (x == null) {}
来源：http://ze.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dr.hnjuh.cn

Go:   if x == nil {}
来源：http://ep.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lk.bjjhwx.cn

C#:   if (x is null) {}
来源：http://qx.shtwfgs.cn

[P07] 防抖与节流
来源：http://nv.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qu.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://td.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pj.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mm.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vl.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cy.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nd.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ey.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://hv.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mm.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kp.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ey.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dk.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vu.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uw.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sa.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zy.panjiajie.cn

================================================================================
来源：http://gn.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zm.hnjuh.cn

================================================================================
来源：http://uk.yuntaijiaju.cn

[Q01] 创建表
来源：http://hq.muxihuayi.cn

CREATE TABLE users (
来源：http://ym.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hg.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://nu.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://ck.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ae.hnjuh.cn

);
来源：http://tj.521024.cn

[Q02] 创建带外键的表
来源：http://ls.huanxung.cn

CREATE TABLE orders (
来源：http://ow.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jj.szsharing.cn

user_id INT NOT NULL,
来源：http://oy.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://oq.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pf.newstarts.cn

);
来源：http://mi.bookmarksfly.cn

[Q03] 增加列
来源：http://wz.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pw.hnjuh.cn

[Q04] 修改列类型
来源：http://xe.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gt.gzmigu.cn

[Q05] 重命名列
来源：http://xt.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zt.shxzukj.cn

[Q06] 删除列
来源：http://kn.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ej.wgjwhj.cn

[Q07] 删除表
来源：http://va.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://cs.521024.cn

[Q08] 创建普通索引
来源：http://iz.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://td.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://av.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ig.muxihuayi.cn

[Q10] 插入单行
来源：http://ms.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qw.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://ya.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ej.521024.cn

[Q12] 插入后取自增 ID
来源：http://ip.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gn.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pp.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://gb.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bo.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://zc.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ku.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ra.9csxet.cn

[Q15] 查询全部
来源：http://fj.shtwfgs.cn

SELECT * FROM users;
来源：http://rm.shtwfgs.cn

[Q16] 查询指定列
来源：http://vg.muxihuayi.cn

SELECT id, name FROM users;
来源：http://yk.hahajie.cn

[Q17] 条件查询
来源：http://uh.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kt.bjjhwx.cn

[Q18] 模糊匹配
来源：http://vp.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mn.bookmarksfly.cn

[Q19] 范围查询
来源：http://tt.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://og.bookmarksfly.cn

[Q20] IN 列表
来源：http://fv.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jm.bjjhwx.cn

[Q21] 空值判断
来源：http://zx.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nn.haigaiapp.cn

[Q22] 排序
来源：http://ul.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://se.panjiajie.cn

[Q23] 分页
来源：http://tk.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gf.lnxyls.cn

[Q24] 去重
来源：http://oe.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://bu.hahajie.cn

[Q25] 只取前 N 条
来源：http://ox.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hb.nszjky.cn

[Q26] 计数
来源：http://cj.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://mf.lnxyls.cn

[Q27] 条件计数
来源：http://km.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vh.szxytkj.cn

[Q28] 求和与平均
来源：http://bu.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bm.chemitech.net.cn

[Q29] 最大最小值
来源：http://fp.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cr.colortex.cn

[Q30] 分组统计
来源：http://dg.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lj.yuexingan06.cn

[Q31] 分组后过滤
来源：http://et.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qi.9csxet.cn

[Q32] 分组拼接字符串
来源：http://tz.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gk.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qv.haigaiapp.cn

[Q33] 多列分组
来源：http://cn.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://la.gzmigu.cn

[Q34] 每组取第一条
来源：http://oy.chemitech.net.cn

SELECT * FROM (
来源：http://zv.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://en.chemitech.net.cn

) t WHERE rn = 1;
来源：http://bk.shxzskj.cn

[Q35] 内连接
来源：http://ru.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yc.huixiangedu.cn

[Q36] 左连接
来源：http://xs.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ix.bjjhwx.cn

[Q37] 右连接
来源：http://yg.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vi.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qj.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wk.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://cn.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xo.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rp.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xr.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eh.huixiangedu.cn

[Q41] 多表连接
来源：http://sm.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vl.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://ii.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://kx.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://av.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://hw.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ql.muxihuayi.cn

[Q43] 标量子查询
来源：http://au.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://go.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://qs.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cm.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://de.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ot.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ys.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cu.hnjuh.cn

[Q47] 与平均值比较
来源：http://re.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ki.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://zf.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oh.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://xl.lnxyls.cn

[Q49] 更新单行
来源：http://dj.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sk.huixinmuqiang.cn

[Q50] 批量更新
来源：http://vm.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ut.muxihuayi.cn

[Q51] 用子查询更新
来源：http://fs.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rp.shtwfgs.cn

[Q52] 删除指定行
来源：http://yi.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://pi.shxzskj.cn

[Q53] 按条件删除
来源：http://zo.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uo.shxzskj.cn

[Q54] 清空表
来源：http://vg.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://jn.asd995.cn

[Q55] 排名（并列占位）
来源：http://vv.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zk.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://dc.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uv.shxzukj.cn

[Q57] 行号
来源：http://bt.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uv.panjiajie.cn

[Q58] 累计求和
来源：http://na.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://as.9csxet.cn

[Q59] 分组内累计
来源：http://al.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cn.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://fu.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ri.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://et.lnxyls.cn

[Q61] 移动平均
来源：http://yy.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://he.shxzskj.cn

[Q62] 分组占比
来源：http://xn.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aw.bookmarksfly.cn

[Q63] 开启事务
来源：http://hn.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://en.nicolike.cn

[Q64] 提交事务
来源：http://ep.asd995.cn

COMMIT;
来源：http://fh.shxzskj.cn

[Q65] 回滚事务
来源：http://tx.lnxyls.cn

ROLLBACK;
来源：http://fo.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://aw.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cd.panjiajie.cn

[Q67] 设置隔离级别
来源：http://mf.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.asd995.cn

[Q68] 保存点
来源：http://ai.hnjuh.cn

SAVEPOINT sp1;
来源：http://yi.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://eg.hnjuh.cn

[Q69] 查看执行计划
来源：http://em.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sv.newstarts.cn

[Q70] 更新统计信息
来源：http://ba.nszjky.cn

ANALYZE TABLE users;
来源：http://el.shxzskj.cn

[Q71] 查看建表语句
来源：http://bq.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rq.gzmigu.cn

[Q72] 查看索引
来源：http://nd.szxytkj.cn

SHOW INDEX FROM users;
来源：http://qz.wgjwhj.cn

[Q73] 查看表状态
来源：http://rc.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sz.gzmigu.cn

[Q74] 强制使用索引
来源：http://si.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://if.bjjhwx.cn

[Q75] 日期格式化
来源：http://tc.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yw.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yw.jianghongdianzi.cn

[Q76] 按天统计
来源：http://sy.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qd.hahajie.cn

[Q77] 时间加减
来源：http://qg.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ts.huixiangedu.cn

[Q78] 当前时间
来源：http://zs.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ak.bjjhwx.cn

[Q79] 字符串拼接
来源：http://yj.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zn.wgjwhj.cn

[Q80] 字符串截取
来源：http://ly.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ky.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://fv.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pd.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://zj.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sf.newstarts.cn

[Q83] 大小写转换
来源：http://sy.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://td.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://ez.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://pl.huanxung.cn

[Q85] 数值取整
来源：http://yc.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dk.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://oo.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qi.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://vo.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gz.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://et.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qh.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://we.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://hl.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jd.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://ay.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gh.szsharing.cn

================================================================================
来源：http://rf.nicolike.cn


<!-- 参考信息 -->