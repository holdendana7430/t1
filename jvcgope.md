代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ce.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ow.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://bc.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://py.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://jt.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yz.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://vt.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://bs.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zf.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ir.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://zp.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fr.chemitech.net.cn

[O06] 使用进程池
来源：http://wp.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fm.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yr.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://pj.colortex.cn

TS:   // child_process / cluster 模块
来源：http://ca.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sl.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zv.lnxyls.cn

Ruby: // fork 块
来源：http://uw.szsharing.cn

C#:   Parallel.For
来源：http://gj.nszjky.cn

================================================================================
来源：http://wt.shtwfgs.cn

P. 常用工具函数
来源：http://jf.hnjuh.cn

================================================================================
来源：http://io.muxihuayi.cn

[P01] 生成 UUID
来源：http://nm.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://gy.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mk.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://ya.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://pl.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://ua.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://ml.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://fs.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://ai.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://no.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zc.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ru.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sx.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ut.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ol.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qd.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dk.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uf.nicolike.cn

[P03] 生成短随机字符串
来源：http://sb.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ln.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ot.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pv.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yu.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hp.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yv.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://us.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sc.huixiangedu.cn

[P04] 求长度
来源：http://xe.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rh.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gv.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ei.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hd.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://hr.newstarts.cn

Go:   len(arr);  len(m)
来源：http://db.lnxyls.cn

Ruby: x.length;  x.size
来源：http://pf.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wr.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://rh.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dt.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ad.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rf.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zb.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cc.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://un.bjjhwx.cn

Ruby: a == b
来源：http://ks.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vz.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nt.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ys.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://of.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dw.521024.cn

TS:   if (x == null) {}
来源：http://tt.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pi.521024.cn

Go:   if x == nil {}
来源：http://gx.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hp.wgjwhj.cn

C#:   if (x is null) {}
来源：http://oy.huanxung.cn

[P07] 防抖与节流
来源：http://iq.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bs.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://kb.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uk.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gk.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mx.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wu.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ok.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sd.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://ou.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lb.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ed.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ys.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bt.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jd.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hf.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jk.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bz.yuexingan06.cn

================================================================================
来源：http://wx.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gu.wgjwhj.cn

================================================================================
来源：http://og.nszjky.cn

[Q01] 创建表
来源：http://so.9csxet.cn

CREATE TABLE users (
来源：http://rt.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qf.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://lo.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://ni.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hu.shtwfgs.cn

);
来源：http://xy.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://ln.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://vk.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qx.gzmigu.cn

user_id INT NOT NULL,
来源：http://ho.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://ri.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aw.bookmarksfly.cn

);
来源：http://hk.muxihuayi.cn

[Q03] 增加列
来源：http://ne.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zu.newstarts.cn

[Q04] 修改列类型
来源：http://we.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jh.nicolike.cn

[Q05] 重命名列
来源：http://pp.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yk.9csxet.cn

[Q06] 删除列
来源：http://fr.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bv.jianghongdianzi.cn

[Q07] 删除表
来源：http://ts.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://kh.huanxung.cn

[Q08] 创建普通索引
来源：http://nz.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bu.newstarts.cn

[Q09] 创建唯一索引
来源：http://in.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nf.9csxet.cn

[Q10] 插入单行
来源：http://ii.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wm.hnjuh.cn

[Q11] 一次插入多行
来源：http://nh.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ge.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://am.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ry.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wt.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://fj.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ox.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://iq.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zw.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nu.panjiajie.cn

[Q15] 查询全部
来源：http://nf.shxzskj.cn

SELECT * FROM users;
来源：http://ek.bookmarksfly.cn

[Q16] 查询指定列
来源：http://qm.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://fq.jianghongdianzi.cn

[Q17] 条件查询
来源：http://yi.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dt.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://rk.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ab.hahajie.cn

[Q19] 范围查询
来源：http://fp.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zo.bookmarksfly.cn

[Q20] IN 列表
来源：http://vt.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xt.shxzukj.cn

[Q21] 空值判断
来源：http://mj.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jv.huixiangedu.cn

[Q22] 排序
来源：http://yb.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uo.haigaiapp.cn

[Q23] 分页
来源：http://qc.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fm.nszjky.cn

[Q24] 去重
来源：http://ap.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://yv.521024.cn

[Q25] 只取前 N 条
来源：http://cr.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nq.jianghongdianzi.cn

[Q26] 计数
来源：http://sn.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://by.lnxyls.cn

[Q27] 条件计数
来源：http://yd.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zh.szxytkj.cn

[Q28] 求和与平均
来源：http://hj.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vc.colortex.cn

[Q29] 最大最小值
来源：http://mw.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rg.yuexingan06.cn

[Q30] 分组统计
来源：http://dv.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zk.gzmigu.cn

[Q31] 分组后过滤
来源：http://qw.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bl.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://vh.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iu.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ft.colortex.cn

[Q33] 多列分组
来源：http://ad.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iv.bjjhwx.cn

[Q34] 每组取第一条
来源：http://aw.szxytkj.cn

SELECT * FROM (
来源：http://wq.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://is.hahajie.cn

) t WHERE rn = 1;
来源：http://xy.chemitech.net.cn

[Q35] 内连接
来源：http://cc.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pj.nszjky.cn

[Q36] 左连接
来源：http://ax.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ev.jctech888.com.cn

[Q37] 右连接
来源：http://wm.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sy.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://il.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ze.colortex.cn

[Q39] 自连接（查上下级）
来源：http://ev.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wx.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tw.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lj.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pj.szsharing.cn

[Q41] 多表连接
来源：http://dn.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://in.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://gz.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://xm.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://yu.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://va.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uk.colortex.cn

[Q43] 标量子查询
来源：http://hq.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nu.newstarts.cn

[Q44] IN 子查询
来源：http://tg.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rf.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://gn.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://su.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ys.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kv.panjiajie.cn

[Q47] 与平均值比较
来源：http://ie.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ez.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://oj.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ju.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://eg.hahajie.cn

[Q49] 更新单行
来源：http://wy.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dv.wgjwhj.cn

[Q50] 批量更新
来源：http://ym.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://us.huixiangedu.cn

[Q51] 用子查询更新
来源：http://ys.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ok.bjjhwx.cn

[Q52] 删除指定行
来源：http://yb.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://pc.muxihuayi.cn

[Q53] 按条件删除
来源：http://fy.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vk.hahajie.cn

[Q54] 清空表
来源：http://vd.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://le.newstarts.cn

[Q55] 排名（并列占位）
来源：http://qa.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gc.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://gk.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uq.wgjwhj.cn

[Q57] 行号
来源：http://xl.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hg.9csxet.cn

[Q58] 累计求和
来源：http://pn.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sm.hnjuh.cn

[Q59] 分组内累计
来源：http://mt.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kh.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://od.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tc.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lw.huixinmuqiang.cn

[Q61] 移动平均
来源：http://ye.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fk.szxytkj.cn

[Q62] 分组占比
来源：http://bn.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ym.colortex.cn

[Q63] 开启事务
来源：http://it.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ix.newstarts.cn

[Q64] 提交事务
来源：http://bz.nszjky.cn

COMMIT;
来源：http://su.lnxyls.cn

[Q65] 回滚事务
来源：http://oq.szxytkj.cn

ROLLBACK;
来源：http://kv.hahajie.cn

[Q66] 行锁查询
来源：http://xc.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iw.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://qg.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://go.gzmigu.cn

[Q68] 保存点
来源：http://ex.521024.cn

SAVEPOINT sp1;
来源：http://nh.colortex.cn

ROLLBACK TO sp1;
来源：http://iy.shtwfgs.cn

[Q69] 查看执行计划
来源：http://fg.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ew.chemitech.net.cn

[Q70] 更新统计信息
来源：http://ps.muxihuayi.cn

ANALYZE TABLE users;
来源：http://ku.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://qk.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kn.gzmigu.cn

[Q72] 查看索引
来源：http://xl.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://fo.panjiajie.cn

[Q73] 查看表状态
来源：http://ro.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xl.szxytkj.cn

[Q74] 强制使用索引
来源：http://xh.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qg.shxzskj.cn

[Q75] 日期格式化
来源：http://ft.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wu.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mn.yuntaijiaju.cn

[Q76] 按天统计
来源：http://ze.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ft.521024.cn

[Q77] 时间加减
来源：http://jv.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wf.yuntaijiaju.cn

[Q78] 当前时间
来源：http://rf.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rh.jctech888.com.cn

[Q79] 字符串拼接
来源：http://la.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zw.shxzskj.cn

[Q80] 字符串截取
来源：http://pg.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iu.huixiangedu.cn

[Q81] 字符串替换
来源：http://iq.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xn.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://rh.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jw.haigaiapp.cn

[Q83] 大小写转换
来源：http://ye.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sx.szsharing.cn

[Q84] 去除首尾空格
来源：http://cy.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://od.yuntaijiaju.cn

[Q85] 数值取整
来源：http://gf.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mm.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://zm.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nf.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://sp.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xo.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://wo.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ur.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fr.nicolike.cn

[Q89] 判断表是否存在
来源：http://ri.haigaiapp.cn


<!-- 参考信息 -->