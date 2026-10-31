代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jt.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lf.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://ye.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fa.szsharing.cn

[O06] 使用进程池
来源：http://ps.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ai.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tg.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://hx.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://jc.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ki.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oa.9csxet.cn

Ruby: // fork 块
来源：http://wd.shxzskj.cn

C#:   Parallel.For
来源：http://vb.newstarts.cn

================================================================================
来源：http://og.shtwfgs.cn

P. 常用工具函数
来源：http://oj.nicolike.cn

================================================================================
来源：http://pu.chemitech.net.cn

[P01] 生成 UUID
来源：http://yn.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://on.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jx.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://za.szsharing.cn

TS:   crypto.randomUUID()
来源：http://ml.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://xd.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://fa.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://lf.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://sw.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://lm.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cc.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tp.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mk.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qw.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uh.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ra.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ol.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hn.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://yg.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mb.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ba.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jv.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://br.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mo.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cc.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lj.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hk.jianghongdianzi.cn

[P04] 求长度
来源：http://uf.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ef.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nw.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xv.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nz.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ej.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://td.shxzskj.cn

Ruby: x.length;  x.size
来源：http://dy.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lx.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://ae.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ss.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sy.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fw.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ny.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rl.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pm.shxzskj.cn

Ruby: a == b
来源：http://yb.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hx.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ca.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wf.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://ai.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kn.huanxung.cn

TS:   if (x == null) {}
来源：http://hh.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ih.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://ne.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xe.chemitech.net.cn

C#:   if (x is null) {}
来源：http://ky.huanxung.cn

[P07] 防抖与节流
来源：http://qk.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uq.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://fc.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qy.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ii.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ml.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jv.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zr.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rl.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://ya.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xo.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ow.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xp.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ck.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ha.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yc.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hh.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ta.muxihuayi.cn

================================================================================
来源：http://ak.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jp.bookmarksfly.cn

================================================================================
来源：http://sw.haigaiapp.cn

[Q01] 创建表
来源：http://bu.asd995.cn

CREATE TABLE users (
来源：http://at.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mf.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://uv.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://la.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://me.bookmarksfly.cn

);
来源：http://vu.gzmigu.cn

[Q02] 创建带外键的表
来源：http://hu.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://fr.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ha.huixiangedu.cn

user_id INT NOT NULL,
来源：http://cg.huanxung.cn

amount DECIMAL(10, 2),
来源：http://ip.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ia.szsharing.cn

);
来源：http://dv.hnjuh.cn

[Q03] 增加列
来源：http://yr.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qo.nicolike.cn

[Q04] 修改列类型
来源：http://wn.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qr.shxzskj.cn

[Q05] 重命名列
来源：http://ga.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wh.yuntaijiaju.cn

[Q06] 删除列
来源：http://vq.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fr.jctech888.com.cn

[Q07] 删除表
来源：http://hi.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://tk.yuexingan06.cn

[Q08] 创建普通索引
来源：http://co.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sf.hnjuh.cn

[Q09] 创建唯一索引
来源：http://sj.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://op.9csxet.cn

[Q10] 插入单行
来源：http://vd.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aj.haigaiapp.cn

[Q11] 一次插入多行
来源：http://bk.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fm.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://uh.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yc.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://do.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://pw.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yw.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://tb.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ot.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kr.szxytkj.cn

[Q15] 查询全部
来源：http://rq.yuexingan06.cn

SELECT * FROM users;
来源：http://sp.lnxyls.cn

[Q16] 查询指定列
来源：http://zp.haigaiapp.cn

SELECT id, name FROM users;
来源：http://yu.gzmigu.cn

[Q17] 条件查询
来源：http://pm.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wq.hnjuh.cn

[Q18] 模糊匹配
来源：http://di.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yz.colortex.cn

[Q19] 范围查询
来源：http://av.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pc.lnxyls.cn

[Q20] IN 列表
来源：http://fn.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nk.jctech888.com.cn

[Q21] 空值判断
来源：http://bi.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sb.chemitech.net.cn

[Q22] 排序
来源：http://jm.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ro.jctech888.com.cn

[Q23] 分页
来源：http://zr.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://df.521024.cn

[Q24] 去重
来源：http://sv.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://uq.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://up.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pc.bookmarksfly.cn

[Q26] 计数
来源：http://yx.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://uy.jctech888.com.cn

[Q27] 条件计数
来源：http://wv.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lu.521024.cn

[Q28] 求和与平均
来源：http://sh.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ih.haigaiapp.cn

[Q29] 最大最小值
来源：http://hk.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sa.szsharing.cn

[Q30] 分组统计
来源：http://dt.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gj.jctech888.com.cn

[Q31] 分组后过滤
来源：http://st.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rc.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://ow.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nt.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nc.bjjhwx.cn

[Q33] 多列分组
来源：http://nb.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tb.muxihuayi.cn

[Q34] 每组取第一条
来源：http://us.chemitech.net.cn

SELECT * FROM (
来源：http://sd.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jh.9csxet.cn

) t WHERE rn = 1;
来源：http://cm.bookmarksfly.cn

[Q35] 内连接
来源：http://bn.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kj.hnjuh.cn

[Q36] 左连接
来源：http://gj.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ns.szxytkj.cn

[Q37] 右连接
来源：http://qs.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xb.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zo.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ug.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://xt.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://es.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wq.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kr.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gj.huixinmuqiang.cn

[Q41] 多表连接
来源：http://yl.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zq.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ue.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://el.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://zz.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://pk.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bh.shxzukj.cn

[Q43] 标量子查询
来源：http://wb.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yn.lnxyls.cn

[Q44] IN 子查询
来源：http://ij.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zy.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://zy.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xq.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wh.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xs.shtwfgs.cn

[Q47] 与平均值比较
来源：http://md.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jd.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://aw.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hs.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://yy.shxzskj.cn

[Q49] 更新单行
来源：http://jf.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rk.muxihuayi.cn

[Q50] 批量更新
来源：http://uj.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mw.chemitech.net.cn

[Q51] 用子查询更新
来源：http://gu.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://px.jctech888.com.cn

[Q52] 删除指定行
来源：http://uy.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://cm.wgjwhj.cn

[Q53] 按条件删除
来源：http://wc.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nj.yuntaijiaju.cn

[Q54] 清空表
来源：http://qv.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://rv.newstarts.cn

[Q55] 排名（并列占位）
来源：http://ps.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wp.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://on.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jo.lnxyls.cn

[Q57] 行号
来源：http://hf.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ku.nszjky.cn

[Q58] 累计求和
来源：http://vv.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mo.wgjwhj.cn

[Q59] 分组内累计
来源：http://wb.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rl.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://io.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yt.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cp.bookmarksfly.cn

[Q61] 移动平均
来源：http://ja.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yv.hahajie.cn

[Q62] 分组占比
来源：http://hb.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dn.huanxung.cn

[Q63] 开启事务
来源：http://uc.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jt.muxihuayi.cn

[Q64] 提交事务
来源：http://kv.yuntaijiaju.cn

COMMIT;
来源：http://gw.bjjhwx.cn

[Q65] 回滚事务
来源：http://te.shxzukj.cn

ROLLBACK;
来源：http://cv.bjjhwx.cn

[Q66] 行锁查询
来源：http://wt.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yh.gzmigu.cn

[Q67] 设置隔离级别
来源：http://xa.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rw.yuntaijiaju.cn

[Q68] 保存点
来源：http://mp.nszjky.cn

SAVEPOINT sp1;
来源：http://ca.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://mx.huixiangedu.cn

[Q69] 查看执行计划
来源：http://vy.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oq.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://qa.chemitech.net.cn

ANALYZE TABLE users;
来源：http://fk.szxytkj.cn

[Q71] 查看建表语句
来源：http://ti.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zs.9csxet.cn

[Q72] 查看索引
来源：http://gx.hnjuh.cn

SHOW INDEX FROM users;
来源：http://si.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ta.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vk.szxytkj.cn

[Q74] 强制使用索引
来源：http://at.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ai.wgjwhj.cn

[Q75] 日期格式化
来源：http://ji.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vk.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ui.newstarts.cn

[Q76] 按天统计
来源：http://da.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gx.521024.cn

[Q77] 时间加减
来源：http://js.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jt.huanxung.cn

[Q78] 当前时间
来源：http://pq.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lo.shxzukj.cn

[Q79] 字符串拼接
来源：http://wx.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kq.chemitech.net.cn

[Q80] 字符串截取
来源：http://sv.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ti.jctech888.com.cn

[Q81] 字符串替换
来源：http://zw.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oe.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://qp.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ti.nszjky.cn

[Q83] 大小写转换
来源：http://du.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fa.9csxet.cn

[Q84] 去除首尾空格
来源：http://gu.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://ur.9csxet.cn

[Q85] 数值取整
来源：http://qa.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yb.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://me.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ur.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ag.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kg.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://ss.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zm.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ui.panjiajie.cn

[Q89] 判断表是否存在
来源：http://bx.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vo.yuexingan06.cn

[Q90] 生成序号列
来源：http://cb.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://st.nszjky.cn

================================================================================
来源：http://vm.gzmigu.cn

R. Bash 专题
来源：http://tr.521024.cn

================================================================================
来源：http://oi.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://ak.jctech888.com.cn

#!/usr/bin/env bash
来源：http://yu.9csxet.cn


<!-- 参考信息 -->