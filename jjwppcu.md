代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://py.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cs.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://go.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://wz.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zt.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ke.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://eb.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://og.bjjhwx.cn

[O06] 使用进程池
来源：http://vr.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hh.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jn.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://pq.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://jd.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ru.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pu.szxytkj.cn

Ruby: // fork 块
来源：http://yz.hnjuh.cn

C#:   Parallel.For
来源：http://ev.chemitech.net.cn

================================================================================
来源：http://pp.szsharing.cn

P. 常用工具函数
来源：http://ac.gzmigu.cn

================================================================================
来源：http://tb.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://xo.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://zy.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dj.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://rz.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://su.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://uf.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://fk.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://sv.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://qg.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://gm.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zf.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ns.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qp.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bv.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ce.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nr.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://df.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xm.huanxung.cn

[P03] 生成短随机字符串
来源：http://og.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cx.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://au.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ir.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ux.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jy.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tx.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://np.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://br.colortex.cn

[P04] 求长度
来源：http://cz.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ae.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gh.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pq.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dj.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://kb.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://xn.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ng.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ui.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://wi.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ja.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mm.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://py.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ol.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rm.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cp.bjjhwx.cn

Ruby: a == b
来源：http://sr.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hv.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vs.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oi.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://um.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ef.yuexingan06.cn

TS:   if (x == null) {}
来源：http://zu.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ne.chemitech.net.cn

Go:   if x == nil {}
来源：http://px.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://as.panjiajie.cn

C#:   if (x is null) {}
来源：http://np.shtwfgs.cn

[P07] 防抖与节流
来源：http://mg.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vi.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://yv.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gr.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://if.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tk.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uk.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rl.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ig.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://co.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sz.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ek.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nb.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uz.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gx.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ft.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hd.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lk.huixinmuqiang.cn

================================================================================
来源：http://uq.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pv.jianghongdianzi.cn

================================================================================
来源：http://tb.hahajie.cn

[Q01] 创建表
来源：http://xe.haigaiapp.cn

CREATE TABLE users (
来源：http://xu.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://an.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://fm.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://jw.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lg.szxytkj.cn

);
来源：http://ln.lnxyls.cn

[Q02] 创建带外键的表
来源：http://ai.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://el.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gr.gzmigu.cn

user_id INT NOT NULL,
来源：http://de.colortex.cn

amount DECIMAL(10, 2),
来源：http://vh.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wx.yuntaijiaju.cn

);
来源：http://of.huanxung.cn

[Q03] 增加列
来源：http://bt.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ji.panjiajie.cn

[Q04] 修改列类型
来源：http://bs.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ws.lnxyls.cn

[Q05] 重命名列
来源：http://dx.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hx.lnxyls.cn

[Q06] 删除列
来源：http://ce.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://th.colortex.cn

[Q07] 删除表
来源：http://di.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://ej.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ix.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hx.szxytkj.cn

[Q09] 创建唯一索引
来源：http://ml.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://va.shxzskj.cn

[Q10] 插入单行
来源：http://dr.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bv.chemitech.net.cn

[Q11] 一次插入多行
来源：http://ax.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dh.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://hr.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jr.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bj.huanxung.cn

[Q13] 忽略重复插入
来源：http://fu.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rq.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://kk.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dl.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oq.yuntaijiaju.cn

[Q15] 查询全部
来源：http://rl.yuntaijiaju.cn

SELECT * FROM users;
来源：http://si.huanxung.cn

[Q16] 查询指定列
来源：http://rm.nszjky.cn

SELECT id, name FROM users;
来源：http://fz.nszjky.cn

[Q17] 条件查询
来源：http://sz.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lm.gzmigu.cn

[Q18] 模糊匹配
来源：http://dq.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ak.shxzukj.cn

[Q19] 范围查询
来源：http://qq.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cc.yuntaijiaju.cn

[Q20] IN 列表
来源：http://nu.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://py.shxzukj.cn

[Q21] 空值判断
来源：http://fd.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gs.9csxet.cn

[Q22] 排序
来源：http://pb.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jk.nszjky.cn

[Q23] 分页
来源：http://mu.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rw.shxzukj.cn

[Q24] 去重
来源：http://sj.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://wu.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://lo.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pk.gzmigu.cn

[Q26] 计数
来源：http://xi.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://bm.jctech888.com.cn

[Q27] 条件计数
来源：http://cv.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ei.hahajie.cn

[Q28] 求和与平均
来源：http://hj.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://po.muxihuayi.cn

[Q29] 最大最小值
来源：http://az.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iu.haigaiapp.cn

[Q30] 分组统计
来源：http://eo.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ik.asd995.cn

[Q31] 分组后过滤
来源：http://sl.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wz.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://vv.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yt.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nl.521024.cn

[Q33] 多列分组
来源：http://nw.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aw.huanxung.cn

[Q34] 每组取第一条
来源：http://tc.lnxyls.cn

SELECT * FROM (
来源：http://no.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qv.huanxung.cn

) t WHERE rn = 1;
来源：http://bu.lnxyls.cn

[Q35] 内连接
来源：http://am.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ud.bjjhwx.cn

[Q36] 左连接
来源：http://ic.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gy.shxzukj.cn

[Q37] 右连接
来源：http://ad.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://if.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://op.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oz.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://cz.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://an.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sn.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vu.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lg.chemitech.net.cn

[Q41] 多表连接
来源：http://ez.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zf.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://fe.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://zz.colortex.cn

[Q42] 连接条件附加过滤
来源：http://yv.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://pl.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qz.huanxung.cn

[Q43] 标量子查询
来源：http://kv.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tp.hnjuh.cn

[Q44] IN 子查询
来源：http://eo.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sl.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://ri.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://im.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ax.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://la.muxihuayi.cn

[Q47] 与平均值比较
来源：http://ct.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qa.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://qq.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wi.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://vn.panjiajie.cn

[Q49] 更新单行
来源：http://pd.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pg.shxzskj.cn

[Q50] 批量更新
来源：http://xp.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cs.hnjuh.cn

[Q51] 用子查询更新
来源：http://di.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iu.nicolike.cn

[Q52] 删除指定行
来源：http://wi.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://co.huixiangedu.cn

[Q53] 按条件删除
来源：http://cn.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sd.muxihuayi.cn

[Q54] 清空表
来源：http://uz.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://mk.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://hu.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hm.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://et.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rb.521024.cn

[Q57] 行号
来源：http://ej.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://so.jianghongdianzi.cn

[Q58] 累计求和
来源：http://bt.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ok.hnjuh.cn

[Q59] 分组内累计
来源：http://wl.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jg.521024.cn

[Q60] 取上一行 / 下一行
来源：http://kq.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ez.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qa.jianghongdianzi.cn

[Q61] 移动平均
来源：http://tr.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jj.shtwfgs.cn

[Q62] 分组占比
来源：http://yj.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tu.shtwfgs.cn

[Q63] 开启事务
来源：http://nr.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wo.newstarts.cn

[Q64] 提交事务
来源：http://tz.hahajie.cn

COMMIT;
来源：http://xo.shtwfgs.cn

[Q65] 回滚事务
来源：http://wz.asd995.cn

ROLLBACK;
来源：http://wl.bookmarksfly.cn

[Q66] 行锁查询
来源：http://jw.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bz.asd995.cn

[Q67] 设置隔离级别
来源：http://nu.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ur.szsharing.cn

[Q68] 保存点
来源：http://sj.shtwfgs.cn

SAVEPOINT sp1;
来源：http://gy.panjiajie.cn

ROLLBACK TO sp1;
来源：http://lk.szsharing.cn

[Q69] 查看执行计划
来源：http://xb.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xd.szxytkj.cn

[Q70] 更新统计信息
来源：http://wf.shxzskj.cn

ANALYZE TABLE users;
来源：http://gc.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://zl.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iq.haigaiapp.cn

[Q72] 查看索引
来源：http://gt.nszjky.cn

SHOW INDEX FROM users;
来源：http://kl.gzmigu.cn

[Q73] 查看表状态
来源：http://hk.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://is.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://qj.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://te.huanxung.cn

[Q75] 日期格式化
来源：http://ag.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dj.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rc.bjjhwx.cn

[Q76] 按天统计
来源：http://vi.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fu.yuntaijiaju.cn

[Q77] 时间加减
来源：http://km.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dl.9csxet.cn

[Q78] 当前时间
来源：http://nl.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mz.asd995.cn

[Q79] 字符串拼接
来源：http://to.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rr.521024.cn

[Q80] 字符串截取
来源：http://vm.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://om.huixiangedu.cn

[Q81] 字符串替换
来源：http://xl.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://km.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://xi.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://le.hnjuh.cn

[Q83] 大小写转换
来源：http://df.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ph.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://rm.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://su.nicolike.cn

[Q85] 数值取整
来源：http://ut.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qv.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://cq.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yb.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://sf.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wt.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://it.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gr.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kd.hahajie.cn

[Q89] 判断表是否存在
来源：http://ai.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hl.nicolike.cn

[Q90] 生成序号列
来源：http://qb.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://db.bookmarksfly.cn

================================================================================
来源：http://ga.jctech888.com.cn


<!-- 参考信息 -->