代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sy.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://fa.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tl.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oi.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fd.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mz.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://pl.521024.cn

[O05] 并发执行并等待全部完成
来源：http://fz.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://ul.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://np.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://cn.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://uz.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ur.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ct.asd995.cn

Ruby: threads.map(&:join)
来源：http://sy.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bu.huanxung.cn

[O06] 使用进程池
来源：http://rc.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ja.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nq.asd995.cn

JS:   // child_process / cluster 模块
来源：http://wz.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ol.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gj.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cs.asd995.cn

Ruby: // fork 块
来源：http://xu.colortex.cn

C#:   Parallel.For
来源：http://ty.9csxet.cn

================================================================================
来源：http://zh.nszjky.cn

P. 常用工具函数
来源：http://pi.nszjky.cn

================================================================================
来源：http://fl.9csxet.cn

[P01] 生成 UUID
来源：http://ro.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://ks.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bo.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://gh.521024.cn

TS:   crypto.randomUUID()
来源：http://wd.521024.cn

Java: UUID.randomUUID().toString()
来源：http://yr.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ve.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://oz.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://zs.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://yg.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wu.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ya.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://co.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qm.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yb.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://on.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cw.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jl.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://sl.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://by.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gq.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ju.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://he.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cq.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fy.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zx.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ww.szsharing.cn

[P04] 求长度
来源：http://oh.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ph.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ce.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pn.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rb.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://bp.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://ev.lnxyls.cn

Ruby: x.length;  x.size
来源：http://vb.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cj.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://bd.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wa.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tm.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vl.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://om.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dk.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://af.nicolike.cn

Ruby: a == b
来源：http://zu.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://li.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lc.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sb.colortex.cn

PHP:  if (empty($x)) {}
来源：http://tv.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ra.shxzukj.cn

TS:   if (x == null) {}
来源：http://ww.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://em.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://bq.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fv.haigaiapp.cn

C#:   if (x is null) {}
来源：http://rg.asd995.cn

[P07] 防抖与节流
来源：http://rk.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kp.521024.cn

PHP:  // 手写时间戳比较
来源：http://ks.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ql.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bc.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xc.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bb.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://id.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zw.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://ml.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vj.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tl.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cx.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xe.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tp.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bj.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jf.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kr.muxihuayi.cn

================================================================================
来源：http://xb.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wj.haigaiapp.cn

================================================================================
来源：http://ki.wgjwhj.cn

[Q01] 创建表
来源：http://pk.hnjuh.cn

CREATE TABLE users (
来源：http://zd.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pg.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://zt.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://bo.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://na.shxzukj.cn

);
来源：http://uv.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://dz.nicolike.cn

CREATE TABLE orders (
来源：http://uv.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wp.newstarts.cn

user_id INT NOT NULL,
来源：http://pl.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://wd.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vo.jianghongdianzi.cn

);
来源：http://di.panjiajie.cn

[Q03] 增加列
来源：http://az.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uu.lnxyls.cn

[Q04] 修改列类型
来源：http://dk.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yw.nszjky.cn

[Q05] 重命名列
来源：http://ha.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ee.shxzskj.cn

[Q06] 删除列
来源：http://bg.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mb.yuntaijiaju.cn

[Q07] 删除表
来源：http://cw.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ha.colortex.cn

[Q08] 创建普通索引
来源：http://pb.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fs.521024.cn

[Q09] 创建唯一索引
来源：http://ne.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bb.gzmigu.cn

[Q10] 插入单行
来源：http://vt.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oa.huixiangedu.cn

[Q11] 一次插入多行
来源：http://pu.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gh.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://bm.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://it.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lm.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://nd.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hv.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://nw.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tl.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rj.wgjwhj.cn

[Q15] 查询全部
来源：http://bc.asd995.cn

SELECT * FROM users;
来源：http://tx.asd995.cn

[Q16] 查询指定列
来源：http://wd.huixiangedu.cn

SELECT id, name FROM users;
来源：http://fb.asd995.cn

[Q17] 条件查询
来源：http://kt.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ph.shxzskj.cn

[Q18] 模糊匹配
来源：http://is.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xu.bjjhwx.cn

[Q19] 范围查询
来源：http://mj.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fj.panjiajie.cn

[Q20] IN 列表
来源：http://vn.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yh.muxihuayi.cn

[Q21] 空值判断
来源：http://yy.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dx.chemitech.net.cn

[Q22] 排序
来源：http://eo.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bw.shxzskj.cn

[Q23] 分页
来源：http://oh.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uc.nicolike.cn

[Q24] 去重
来源：http://le.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://rr.shxzskj.cn

[Q25] 只取前 N 条
来源：http://iv.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ug.nszjky.cn

[Q26] 计数
来源：http://yu.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://lj.panjiajie.cn

[Q27] 条件计数
来源：http://hw.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kj.wgjwhj.cn

[Q28] 求和与平均
来源：http://tt.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bb.chemitech.net.cn

[Q29] 最大最小值
来源：http://mq.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ln.hnjuh.cn

[Q30] 分组统计
来源：http://vj.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yu.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://mi.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nj.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://nq.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tu.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kx.lnxyls.cn

[Q33] 多列分组
来源：http://ya.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tp.huixiangedu.cn

[Q34] 每组取第一条
来源：http://pd.newstarts.cn

SELECT * FROM (
来源：http://lc.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oo.nszjky.cn

) t WHERE rn = 1;
来源：http://ki.bjjhwx.cn

[Q35] 内连接
来源：http://sh.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nj.panjiajie.cn

[Q36] 左连接
来源：http://zw.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oi.haigaiapp.cn

[Q37] 右连接
来源：http://of.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xu.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vm.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qt.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://zt.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fw.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gx.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uv.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hd.nszjky.cn

[Q41] 多表连接
来源：http://ya.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bs.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://la.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://zb.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://em.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://xn.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ru.hnjuh.cn

[Q43] 标量子查询
来源：http://do.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ji.lnxyls.cn

[Q44] IN 子查询
来源：http://rl.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://we.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://ei.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vy.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vo.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zs.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://ld.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nd.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://pt.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jl.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://xo.nicolike.cn

[Q49] 更新单行
来源：http://fq.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lj.jctech888.com.cn

[Q50] 批量更新
来源：http://uw.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ea.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://mu.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ky.huixiangedu.cn

[Q52] 删除指定行
来源：http://gz.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://co.szxytkj.cn

[Q53] 按条件删除
来源：http://yw.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ow.colortex.cn

[Q54] 清空表
来源：http://wi.huanxung.cn

TRUNCATE TABLE logs;
来源：http://fc.9csxet.cn

[Q55] 排名（并列占位）
来源：http://ng.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dm.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://no.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://us.shxzukj.cn

[Q57] 行号
来源：http://bp.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://im.panjiajie.cn

[Q58] 累计求和
来源：http://au.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lo.nszjky.cn

[Q59] 分组内累计
来源：http://kz.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pb.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://mh.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ur.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wb.jianghongdianzi.cn

[Q61] 移动平均
来源：http://st.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://py.huanxung.cn

[Q62] 分组占比
来源：http://hn.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pm.bjjhwx.cn

[Q63] 开启事务
来源：http://bv.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qv.jctech888.com.cn

[Q64] 提交事务
来源：http://at.asd995.cn

COMMIT;
来源：http://sj.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://yh.shxzskj.cn

ROLLBACK;
来源：http://iz.lnxyls.cn

[Q66] 行锁查询
来源：http://rg.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ch.9csxet.cn

[Q67] 设置隔离级别
来源：http://mt.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wv.chemitech.net.cn

[Q68] 保存点
来源：http://cg.521024.cn

SAVEPOINT sp1;
来源：http://ax.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://mt.521024.cn

[Q69] 查看执行计划
来源：http://es.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zb.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://vf.hnjuh.cn

ANALYZE TABLE users;
来源：http://ce.huanxung.cn

[Q71] 查看建表语句
来源：http://hf.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://al.haigaiapp.cn

[Q72] 查看索引
来源：http://uq.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://et.nicolike.cn

[Q73] 查看表状态
来源：http://qn.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gb.wgjwhj.cn

[Q74] 强制使用索引
来源：http://jz.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oy.szsharing.cn

[Q75] 日期格式化
来源：http://ma.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hr.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sc.szxytkj.cn

[Q76] 按天统计
来源：http://ds.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wt.yuexingan06.cn

[Q77] 时间加减
来源：http://my.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ey.bjjhwx.cn

[Q78] 当前时间
来源：http://vx.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ih.asd995.cn

[Q79] 字符串拼接
来源：http://yi.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qj.shxzukj.cn

[Q80] 字符串截取
来源：http://ww.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rk.bjjhwx.cn

[Q81] 字符串替换
来源：http://tu.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sc.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://gv.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cf.haigaiapp.cn

[Q83] 大小写转换
来源：http://yj.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wx.hnjuh.cn

[Q84] 去除首尾空格
来源：http://st.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://fv.521024.cn

[Q85] 数值取整
来源：http://ep.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lr.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://lg.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ot.colortex.cn

[Q87] JSON 字段做条件
来源：http://gp.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ji.shxzukj.cn


<!-- 参考信息 -->