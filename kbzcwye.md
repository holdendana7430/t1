代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yu.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hy.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://se.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://ff.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://nd.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zb.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://jl.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://fi.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bf.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ro.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://zo.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fn.hahajie.cn

[O06] 使用进程池
来源：http://zq.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tz.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bk.colortex.cn

JS:   // child_process / cluster 模块
来源：http://qd.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://si.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hu.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hy.hnjuh.cn

Ruby: // fork 块
来源：http://le.asd995.cn

C#:   Parallel.For
来源：http://ue.muxihuayi.cn

================================================================================
来源：http://mp.shxzukj.cn

P. 常用工具函数
来源：http://mh.yuexingan06.cn

================================================================================
来源：http://ap.asd995.cn

[P01] 生成 UUID
来源：http://jq.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://ya.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://to.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://ob.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://bl.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://ns.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://pg.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://xz.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://gm.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ni.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lw.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mx.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qj.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cb.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dx.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oh.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pc.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bs.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://is.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://md.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mq.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yi.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qx.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uh.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pz.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xx.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dd.gzmigu.cn

[P04] 求长度
来源：http://ne.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qt.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cv.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://of.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://va.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://vg.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://sq.asd995.cn

Ruby: x.length;  x.size
来源：http://my.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hh.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://ct.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ia.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://it.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gv.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mp.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jl.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nz.hnjuh.cn

Ruby: a == b
来源：http://fs.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fj.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vo.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ms.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://tf.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yg.haigaiapp.cn

TS:   if (x == null) {}
来源：http://yd.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://un.nszjky.cn

Go:   if x == nil {}
来源：http://nu.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ww.nszjky.cn

C#:   if (x is null) {}
来源：http://dy.9csxet.cn

[P07] 防抖与节流
来源：http://sm.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eg.colortex.cn

PHP:  // 手写时间戳比较
来源：http://to.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rd.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gw.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mk.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fk.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://br.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ub.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://de.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lm.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ke.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qf.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ce.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xs.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ly.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tk.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pg.yuntaijiaju.cn

================================================================================
来源：http://in.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xi.asd995.cn

================================================================================
来源：http://gd.hahajie.cn

[Q01] 创建表
来源：http://qg.wgjwhj.cn

CREATE TABLE users (
来源：http://gc.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oq.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://be.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://qa.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kv.521024.cn

);
来源：http://el.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://pr.huanxung.cn

CREATE TABLE orders (
来源：http://bi.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tz.gzmigu.cn

user_id INT NOT NULL,
来源：http://ql.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://ds.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bf.wgjwhj.cn

);
来源：http://uq.9csxet.cn

[Q03] 增加列
来源：http://mc.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wj.haigaiapp.cn

[Q04] 修改列类型
来源：http://yu.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jc.haigaiapp.cn

[Q05] 重命名列
来源：http://wn.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://do.shxzskj.cn

[Q06] 删除列
来源：http://qa.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jq.bookmarksfly.cn

[Q07] 删除表
来源：http://db.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://um.shxzskj.cn

[Q08] 创建普通索引
来源：http://sx.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kq.newstarts.cn

[Q09] 创建唯一索引
来源：http://rw.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uv.huixinmuqiang.cn

[Q10] 插入单行
来源：http://gz.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://an.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://fq.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nh.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ku.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dp.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://es.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://ok.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://px.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://gq.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wa.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qy.gzmigu.cn

[Q15] 查询全部
来源：http://jy.nicolike.cn

SELECT * FROM users;
来源：http://zs.shxzskj.cn

[Q16] 查询指定列
来源：http://iq.jctech888.com.cn

SELECT id, name FROM users;
来源：http://sj.wgjwhj.cn

[Q17] 条件查询
来源：http://ak.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iv.9csxet.cn

[Q18] 模糊匹配
来源：http://pl.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fw.wgjwhj.cn

[Q19] 范围查询
来源：http://vo.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://th.shxzukj.cn

[Q20] IN 列表
来源：http://gr.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sn.haigaiapp.cn

[Q21] 空值判断
来源：http://iq.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cw.szxytkj.cn

[Q22] 排序
来源：http://ss.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wz.gzmigu.cn

[Q23] 分页
来源：http://jd.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cd.asd995.cn

[Q24] 去重
来源：http://lq.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://zv.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://mo.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://az.colortex.cn

[Q26] 计数
来源：http://ig.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://yg.jctech888.com.cn

[Q27] 条件计数
来源：http://bt.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oa.szxytkj.cn

[Q28] 求和与平均
来源：http://bw.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://np.wgjwhj.cn

[Q29] 最大最小值
来源：http://xk.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lv.haigaiapp.cn

[Q30] 分组统计
来源：http://yi.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pz.nszjky.cn

[Q31] 分组后过滤
来源：http://qe.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yp.szsharing.cn

[Q32] 分组拼接字符串
来源：http://rn.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cp.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ph.newstarts.cn

[Q33] 多列分组
来源：http://zb.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rg.asd995.cn

[Q34] 每组取第一条
来源：http://tj.nszjky.cn

SELECT * FROM (
来源：http://em.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yc.shtwfgs.cn

) t WHERE rn = 1;
来源：http://vj.colortex.cn

[Q35] 内连接
来源：http://ow.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://om.panjiajie.cn

[Q36] 左连接
来源：http://mv.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://na.huixiangedu.cn

[Q37] 右连接
来源：http://ch.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wc.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lw.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://di.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://ww.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://db.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ql.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tn.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fq.shtwfgs.cn

[Q41] 多表连接
来源：http://gk.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xy.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ou.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://ig.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://vt.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://na.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fg.shtwfgs.cn

[Q43] 标量子查询
来源：http://iu.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ay.wgjwhj.cn

[Q44] IN 子查询
来源：http://ux.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zk.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://xa.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ue.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cv.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://da.hahajie.cn

[Q47] 与平均值比较
来源：http://jb.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wb.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://pf.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oz.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://tb.hahajie.cn

[Q49] 更新单行
来源：http://as.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lt.nszjky.cn

[Q50] 批量更新
来源：http://tb.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zu.chemitech.net.cn

[Q51] 用子查询更新
来源：http://ev.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wx.shxzukj.cn

[Q52] 删除指定行
来源：http://mw.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://fu.lnxyls.cn

[Q53] 按条件删除
来源：http://yc.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://de.yuntaijiaju.cn

[Q54] 清空表
来源：http://nm.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://tp.nicolike.cn

[Q55] 排名（并列占位）
来源：http://yb.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sy.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://gj.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xn.huixiangedu.cn

[Q57] 行号
来源：http://dw.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gp.bookmarksfly.cn

[Q58] 累计求和
来源：http://ba.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dd.521024.cn

[Q59] 分组内累计
来源：http://zv.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rj.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://us.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rv.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yr.bjjhwx.cn

[Q61] 移动平均
来源：http://ye.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pz.lnxyls.cn

[Q62] 分组占比
来源：http://iv.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gj.szxytkj.cn

[Q63] 开启事务
来源：http://ya.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yn.bjjhwx.cn

[Q64] 提交事务
来源：http://xc.lnxyls.cn

COMMIT;
来源：http://vy.nszjky.cn

[Q65] 回滚事务
来源：http://fe.jianghongdianzi.cn

ROLLBACK;
来源：http://gz.bookmarksfly.cn

[Q66] 行锁查询
来源：http://cg.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wa.hnjuh.cn

[Q67] 设置隔离级别
来源：http://ki.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dt.chemitech.net.cn

[Q68] 保存点
来源：http://bl.9csxet.cn

SAVEPOINT sp1;
来源：http://hz.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://kj.szsharing.cn

[Q69] 查看执行计划
来源：http://fn.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ro.hahajie.cn

[Q70] 更新统计信息
来源：http://ho.muxihuayi.cn

ANALYZE TABLE users;
来源：http://of.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://od.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ef.haigaiapp.cn

[Q72] 查看索引
来源：http://id.shxzskj.cn

SHOW INDEX FROM users;
来源：http://et.hahajie.cn

[Q73] 查看表状态
来源：http://tp.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jk.jctech888.com.cn

[Q74] 强制使用索引
来源：http://wp.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nq.colortex.cn

[Q75] 日期格式化
来源：http://kv.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://so.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nx.shxzukj.cn

[Q76] 按天统计
来源：http://hr.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://np.colortex.cn

[Q77] 时间加减
来源：http://uq.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jx.szsharing.cn

[Q78] 当前时间
来源：http://mg.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vu.wgjwhj.cn

[Q79] 字符串拼接
来源：http://vl.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://br.9csxet.cn

[Q80] 字符串截取
来源：http://ih.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://py.wgjwhj.cn

[Q81] 字符串替换
来源：http://ow.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fg.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://dx.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iw.chemitech.net.cn

[Q83] 大小写转换
来源：http://sv.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fa.521024.cn

[Q84] 去除首尾空格
来源：http://gj.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://oh.muxihuayi.cn

[Q85] 数值取整
来源：http://it.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yi.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://ao.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ig.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://kl.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wg.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://pw.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jz.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cu.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://fz.chemitech.net.cn


<!-- 参考信息 -->