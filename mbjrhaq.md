代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dv.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kx.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://no.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://tg.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://tf.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qw.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ow.colortex.cn

TS:   await Promise.all(tasks)
来源：http://yo.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://er.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cs.hahajie.cn

Ruby: threads.map(&:join)
来源：http://by.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://su.huanxung.cn

[O06] 使用进程池
来源：http://lo.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ub.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ow.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://xc.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://kc.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ic.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oj.shxzukj.cn

Ruby: // fork 块
来源：http://le.shtwfgs.cn

C#:   Parallel.For
来源：http://no.chemitech.net.cn

================================================================================
来源：http://bw.asd995.cn

P. 常用工具函数
来源：http://wa.9csxet.cn

================================================================================
来源：http://tj.shxzskj.cn

[P01] 生成 UUID
来源：http://ie.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://jj.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ic.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://va.nszjky.cn

TS:   crypto.randomUUID()
来源：http://cp.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://gq.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://au.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://jl.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://dp.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://sd.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://as.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qh.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mh.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ww.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ut.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ro.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://te.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://as.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://fd.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bl.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pp.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xb.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zy.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vg.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wh.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ql.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wj.huixinmuqiang.cn

[P04] 求长度
来源：http://ym.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://if.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gx.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://du.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://si.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://rc.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://tg.hahajie.cn

Ruby: x.length;  x.size
来源：http://vt.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rw.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://mi.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pw.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://do.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://za.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wk.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dz.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ln.shxzskj.cn

Ruby: a == b
来源：http://qi.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rx.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nc.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vx.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://bf.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nl.asd995.cn

TS:   if (x == null) {}
来源：http://qy.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qj.wgjwhj.cn

Go:   if x == nil {}
来源：http://yz.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qj.hnjuh.cn

C#:   if (x is null) {}
来源：http://lg.muxihuayi.cn

[P07] 防抖与节流
来源：http://fh.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ow.colortex.cn

PHP:  // 手写时间戳比较
来源：http://cr.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://up.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rd.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xp.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zi.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hs.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pi.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ab.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fk.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yq.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xq.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ss.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lw.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xl.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lq.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://al.9csxet.cn

================================================================================
来源：http://dy.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ow.yuntaijiaju.cn

================================================================================
来源：http://lz.szsharing.cn

[Q01] 创建表
来源：http://mh.shxzukj.cn

CREATE TABLE users (
来源：http://rj.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ui.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://ox.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://mv.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://on.bookmarksfly.cn

);
来源：http://ni.szsharing.cn

[Q02] 创建带外键的表
来源：http://da.newstarts.cn

CREATE TABLE orders (
来源：http://sg.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://le.gzmigu.cn

user_id INT NOT NULL,
来源：http://ia.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://og.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ck.panjiajie.cn

);
来源：http://uq.hnjuh.cn

[Q03] 增加列
来源：http://pm.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oz.szsharing.cn

[Q04] 修改列类型
来源：http://za.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ln.szsharing.cn

[Q05] 重命名列
来源：http://ig.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gb.huixiangedu.cn

[Q06] 删除列
来源：http://st.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rm.asd995.cn

[Q07] 删除表
来源：http://ka.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://bd.wgjwhj.cn

[Q08] 创建普通索引
来源：http://fa.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yp.shxzskj.cn

[Q09] 创建唯一索引
来源：http://fj.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mi.yuexingan06.cn

[Q10] 插入单行
来源：http://nw.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ii.szsharing.cn

[Q11] 一次插入多行
来源：http://yf.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ki.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://wp.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fm.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jb.newstarts.cn

[Q13] 忽略重复插入
来源：http://ig.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fr.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://bd.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lw.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://il.hnjuh.cn

[Q15] 查询全部
来源：http://mi.hahajie.cn

SELECT * FROM users;
来源：http://bn.gzmigu.cn

[Q16] 查询指定列
来源：http://kv.newstarts.cn

SELECT id, name FROM users;
来源：http://dl.gzmigu.cn

[Q17] 条件查询
来源：http://ag.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ti.hnjuh.cn

[Q18] 模糊匹配
来源：http://cl.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fw.huanxung.cn

[Q19] 范围查询
来源：http://yq.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dn.huanxung.cn

[Q20] IN 列表
来源：http://ew.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xn.newstarts.cn

[Q21] 空值判断
来源：http://xv.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://si.muxihuayi.cn

[Q22] 排序
来源：http://pg.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://at.panjiajie.cn

[Q23] 分页
来源：http://aj.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fq.huixinmuqiang.cn

[Q24] 去重
来源：http://mm.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://pt.lnxyls.cn

[Q25] 只取前 N 条
来源：http://cx.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ln.szsharing.cn

[Q26] 计数
来源：http://ke.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://bt.shxzukj.cn

[Q27] 条件计数
来源：http://ys.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bv.hahajie.cn

[Q28] 求和与平均
来源：http://ye.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vc.521024.cn

[Q29] 最大最小值
来源：http://kj.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xk.huixinmuqiang.cn

[Q30] 分组统计
来源：http://cw.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nm.huanxung.cn

[Q31] 分组后过滤
来源：http://kl.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xe.hahajie.cn

[Q32] 分组拼接字符串
来源：http://ye.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tw.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pk.jianghongdianzi.cn

[Q33] 多列分组
来源：http://gj.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vb.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://ow.shxzskj.cn

SELECT * FROM (
来源：http://xe.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cn.newstarts.cn

) t WHERE rn = 1;
来源：http://la.hnjuh.cn

[Q35] 内连接
来源：http://jj.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vb.szsharing.cn

[Q36] 左连接
来源：http://ad.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://np.wgjwhj.cn

[Q37] 右连接
来源：http://no.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xe.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nm.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mw.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://sw.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jx.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://km.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ho.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uw.nszjky.cn

[Q41] 多表连接
来源：http://am.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hr.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://dc.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://ws.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://ks.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://rp.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eg.jctech888.com.cn

[Q43] 标量子查询
来源：http://gd.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gr.nicolike.cn

[Q44] IN 子查询
来源：http://jz.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://et.colortex.cn

[Q45] EXISTS 判断存在
来源：http://oy.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gy.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pz.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xg.9csxet.cn

[Q47] 与平均值比较
来源：http://ue.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ua.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://uq.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xz.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://im.shxzskj.cn

[Q49] 更新单行
来源：http://jc.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ch.huanxung.cn

[Q50] 批量更新
来源：http://gd.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ek.9csxet.cn

[Q51] 用子查询更新
来源：http://bg.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hy.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://jn.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://nc.bookmarksfly.cn

[Q53] 按条件删除
来源：http://pd.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tl.9csxet.cn

[Q54] 清空表
来源：http://hx.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://sr.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://ko.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qy.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://py.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ij.9csxet.cn

[Q57] 行号
来源：http://xs.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kz.bjjhwx.cn

[Q58] 累计求和
来源：http://zu.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dq.gzmigu.cn

[Q59] 分组内累计
来源：http://mz.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rn.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://ev.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aw.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ac.chemitech.net.cn

[Q61] 移动平均
来源：http://yc.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sr.szsharing.cn

[Q62] 分组占比
来源：http://qm.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kl.shxzukj.cn

[Q63] 开启事务
来源：http://kp.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mk.szxytkj.cn

[Q64] 提交事务
来源：http://be.bookmarksfly.cn

COMMIT;
来源：http://vk.chemitech.net.cn

[Q65] 回滚事务
来源：http://rk.jctech888.com.cn

ROLLBACK;
来源：http://sd.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://bg.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wj.521024.cn

[Q67] 设置隔离级别
来源：http://pt.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gd.yuntaijiaju.cn

[Q68] 保存点
来源：http://to.asd995.cn

SAVEPOINT sp1;
来源：http://xn.hahajie.cn

ROLLBACK TO sp1;
来源：http://az.chemitech.net.cn

[Q69] 查看执行计划
来源：http://il.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kh.gzmigu.cn

[Q70] 更新统计信息
来源：http://rf.shxzukj.cn

ANALYZE TABLE users;
来源：http://ko.szsharing.cn

[Q71] 查看建表语句
来源：http://am.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hr.huanxung.cn

[Q72] 查看索引
来源：http://mn.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://qq.hahajie.cn

[Q73] 查看表状态
来源：http://mm.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://it.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://im.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hj.bookmarksfly.cn

[Q75] 日期格式化
来源：http://ku.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ch.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wh.hahajie.cn

[Q76] 按天统计
来源：http://ar.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ww.chemitech.net.cn

[Q77] 时间加减
来源：http://ax.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ur.colortex.cn

[Q78] 当前时间
来源：http://jj.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uk.haigaiapp.cn

[Q79] 字符串拼接
来源：http://rg.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bp.shxzskj.cn

[Q80] 字符串截取
来源：http://ej.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wx.nicolike.cn

[Q81] 字符串替换
来源：http://tu.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jc.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://fb.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ql.haigaiapp.cn

[Q83] 大小写转换
来源：http://ko.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://io.nicolike.cn

[Q84] 去除首尾空格
来源：http://cm.521024.cn

SELECT TRIM(name) FROM users;
来源：http://xy.bjjhwx.cn

[Q85] 数值取整
来源：http://og.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://av.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://po.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rl.nicolike.cn

[Q87] JSON 字段做条件
来源：http://qo.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mv.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://pg.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sq.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rm.9csxet.cn

[Q89] 判断表是否存在
来源：http://hb.bookmarksfly.cn


<!-- 参考信息 -->