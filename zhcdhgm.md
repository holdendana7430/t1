代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xz.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wr.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://xb.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://nv.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://lf.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mo.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://ez.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://rl.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ff.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ia.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://pc.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ex.asd995.cn

[O06] 使用进程池
来源：http://qf.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lg.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dz.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://pi.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://sr.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nf.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ux.yuexingan06.cn

Ruby: // fork 块
来源：http://gj.huanxung.cn

C#:   Parallel.For
来源：http://hx.gzmigu.cn

================================================================================
来源：http://ko.gzmigu.cn

P. 常用工具函数
来源：http://jt.szsharing.cn

================================================================================
来源：http://ut.chemitech.net.cn

[P01] 生成 UUID
来源：http://rl.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://xh.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kc.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://rk.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://of.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://nr.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://ld.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://cf.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://km.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://rk.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ie.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://me.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ae.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://in.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bv.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://su.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xj.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zb.hnjuh.cn

[P03] 生成短随机字符串
来源：http://ke.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ww.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ys.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pm.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wm.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tf.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://df.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gv.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dy.jianghongdianzi.cn

[P04] 求长度
来源：http://zw.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://as.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kf.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qv.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vr.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://eq.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://dl.lnxyls.cn

Ruby: x.length;  x.size
来源：http://kb.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bn.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ca.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qj.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ow.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gl.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hj.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xf.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yv.jianghongdianzi.cn

Ruby: a == b
来源：http://mb.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ed.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vw.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://al.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://uf.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nq.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://mb.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xk.nicolike.cn

Go:   if x == nil {}
来源：http://sc.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ww.newstarts.cn

C#:   if (x is null) {}
来源：http://aw.chemitech.net.cn

[P07] 防抖与节流
来源：http://xd.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nu.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://rt.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vv.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ph.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ti.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nr.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eo.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nj.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://cm.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iy.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vn.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hl.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jo.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qn.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cv.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rd.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ts.lnxyls.cn

================================================================================
来源：http://ma.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bb.huixinmuqiang.cn

================================================================================
来源：http://mm.szxytkj.cn

[Q01] 创建表
来源：http://ye.shtwfgs.cn

CREATE TABLE users (
来源：http://pu.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sr.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://lo.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://qk.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hp.nicolike.cn

);
来源：http://rq.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://oe.521024.cn

CREATE TABLE orders (
来源：http://kt.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pe.newstarts.cn

user_id INT NOT NULL,
来源：http://lq.9csxet.cn

amount DECIMAL(10, 2),
来源：http://cx.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ae.nicolike.cn

);
来源：http://dx.hahajie.cn

[Q03] 增加列
来源：http://tp.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fi.yuexingan06.cn

[Q04] 修改列类型
来源：http://as.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sn.jianghongdianzi.cn

[Q05] 重命名列
来源：http://jm.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cu.nszjky.cn

[Q06] 删除列
来源：http://ud.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ht.shxzukj.cn

[Q07] 删除表
来源：http://qq.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://qd.bjjhwx.cn

[Q08] 创建普通索引
来源：http://nj.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pl.gzmigu.cn

[Q09] 创建唯一索引
来源：http://bk.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nl.szxytkj.cn

[Q10] 插入单行
来源：http://cs.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lv.wgjwhj.cn

[Q11] 一次插入多行
来源：http://er.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://de.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://ga.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fy.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kk.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://gq.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nm.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://dl.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rw.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cd.bookmarksfly.cn

[Q15] 查询全部
来源：http://xf.newstarts.cn

SELECT * FROM users;
来源：http://cr.chemitech.net.cn

[Q16] 查询指定列
来源：http://xj.huanxung.cn

SELECT id, name FROM users;
来源：http://sz.lnxyls.cn

[Q17] 条件查询
来源：http://cg.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wr.shxzskj.cn

[Q18] 模糊匹配
来源：http://ew.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fe.haigaiapp.cn

[Q19] 范围查询
来源：http://ec.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sn.yuexingan06.cn

[Q20] IN 列表
来源：http://yv.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pt.huanxung.cn

[Q21] 空值判断
来源：http://rc.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iz.jctech888.com.cn

[Q22] 排序
来源：http://lb.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uv.gzmigu.cn

[Q23] 分页
来源：http://ju.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gf.gzmigu.cn

[Q24] 去重
来源：http://zf.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://gy.nicolike.cn

[Q25] 只取前 N 条
来源：http://sj.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dw.yuexingan06.cn

[Q26] 计数
来源：http://fx.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://ey.colortex.cn

[Q27] 条件计数
来源：http://ef.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sa.jctech888.com.cn

[Q28] 求和与平均
来源：http://zc.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://en.shxzskj.cn

[Q29] 最大最小值
来源：http://qp.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kx.muxihuayi.cn

[Q30] 分组统计
来源：http://oy.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mb.asd995.cn

[Q31] 分组后过滤
来源：http://ng.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ds.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://mk.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sp.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fw.panjiajie.cn

[Q33] 多列分组
来源：http://at.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sw.521024.cn

[Q34] 每组取第一条
来源：http://nn.szxytkj.cn

SELECT * FROM (
来源：http://yz.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fc.huanxung.cn

) t WHERE rn = 1;
来源：http://rs.nicolike.cn

[Q35] 内连接
来源：http://ji.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gt.9csxet.cn

[Q36] 左连接
来源：http://fs.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vs.muxihuayi.cn

[Q37] 右连接
来源：http://py.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hn.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zo.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qp.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://ti.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wu.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kx.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://io.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yt.9csxet.cn

[Q41] 多表连接
来源：http://pc.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uz.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://rs.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://qx.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://dx.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://kn.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nu.nicolike.cn

[Q43] 标量子查询
来源：http://bb.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lx.521024.cn

[Q44] IN 子查询
来源：http://me.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ao.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://ag.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ec.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ql.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uw.nicolike.cn

[Q47] 与平均值比较
来源：http://eb.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xb.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://bi.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ze.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://kl.nicolike.cn

[Q49] 更新单行
来源：http://wg.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yv.jianghongdianzi.cn

[Q50] 批量更新
来源：http://sz.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ez.hnjuh.cn

[Q51] 用子查询更新
来源：http://re.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kg.gzmigu.cn

[Q52] 删除指定行
来源：http://lw.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://gf.gzmigu.cn

[Q53] 按条件删除
来源：http://bv.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ca.colortex.cn

[Q54] 清空表
来源：http://vv.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://ji.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://ay.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sq.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://nb.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hf.szsharing.cn

[Q57] 行号
来源：http://ou.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hj.shxzskj.cn

[Q58] 累计求和
来源：http://ej.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oh.lnxyls.cn

[Q59] 分组内累计
来源：http://vl.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zi.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://yz.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qy.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nb.muxihuayi.cn

[Q61] 移动平均
来源：http://je.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ds.huixinmuqiang.cn

[Q62] 分组占比
来源：http://eg.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gl.lnxyls.cn

[Q63] 开启事务
来源：http://lc.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ab.szsharing.cn

[Q64] 提交事务
来源：http://yi.haigaiapp.cn

COMMIT;
来源：http://wn.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://xj.yuntaijiaju.cn

ROLLBACK;
来源：http://lt.huanxung.cn

[Q66] 行锁查询
来源：http://wx.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ud.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://dg.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zh.yuntaijiaju.cn

[Q68] 保存点
来源：http://zf.bjjhwx.cn

SAVEPOINT sp1;
来源：http://cu.asd995.cn

ROLLBACK TO sp1;
来源：http://fz.szsharing.cn

[Q69] 查看执行计划
来源：http://ud.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jl.shxzskj.cn

[Q70] 更新统计信息
来源：http://kc.9csxet.cn

ANALYZE TABLE users;
来源：http://rr.szxytkj.cn

[Q71] 查看建表语句
来源：http://ac.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bl.jianghongdianzi.cn

[Q72] 查看索引
来源：http://gl.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://ik.nicolike.cn

[Q73] 查看表状态
来源：http://fh.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pb.huixiangedu.cn

[Q74] 强制使用索引
来源：http://fo.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mh.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://wf.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lf.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://za.yuntaijiaju.cn

[Q76] 按天统计
来源：http://wl.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nj.huixiangedu.cn

[Q77] 时间加减
来源：http://st.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dq.panjiajie.cn

[Q78] 当前时间
来源：http://hc.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gw.chemitech.net.cn

[Q79] 字符串拼接
来源：http://qd.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://za.newstarts.cn

[Q80] 字符串截取
来源：http://kp.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uk.lnxyls.cn

[Q81] 字符串替换
来源：http://mb.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wq.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://ij.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dt.panjiajie.cn

[Q83] 大小写转换
来源：http://du.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bx.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://qe.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://bx.yuexingan06.cn

[Q85] 数值取整
来源：http://lh.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jc.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://zd.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fy.asd995.cn

[Q87] JSON 字段做条件
来源：http://rq.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ad.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://rb.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uh.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ir.newstarts.cn

[Q89] 判断表是否存在
来源：http://on.wgjwhj.cn


<!-- 参考信息 -->