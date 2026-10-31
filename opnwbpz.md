代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zw.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://xx.lnxyls.cn

Py:   with lock: shared += 1
来源：http://hc.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ea.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jc.colortex.cn

TS:   // 同 JS
来源：http://ul.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://bp.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xy.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xl.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://zg.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://up.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://zv.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cw.huanxung.cn

JS:   async function f() { await g(); }
来源：http://mg.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://or.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://id.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eu.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ji.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://nr.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://hm.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://fb.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dt.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://uc.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://iv.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://in.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lu.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://sf.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mo.huixiangedu.cn

[O06] 使用进程池
来源：http://yd.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qp.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wf.asd995.cn

JS:   // child_process / cluster 模块
来源：http://lu.521024.cn

TS:   // child_process / cluster 模块
来源：http://hl.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ss.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mx.bjjhwx.cn

Ruby: // fork 块
来源：http://ne.9csxet.cn

C#:   Parallel.For
来源：http://ag.jianghongdianzi.cn

================================================================================
来源：http://jk.huixiangedu.cn

P. 常用工具函数
来源：http://jr.hahajie.cn

================================================================================
来源：http://nc.bjjhwx.cn

[P01] 生成 UUID
来源：http://zh.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://la.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ho.huanxung.cn

JS:   crypto.randomUUID()
来源：http://fi.colortex.cn

TS:   crypto.randomUUID()
来源：http://ko.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://on.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://do.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://fv.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://mj.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://hy.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ck.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rx.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wr.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nq.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jw.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zu.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jm.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wb.lnxyls.cn

[P03] 生成短随机字符串
来源：http://xj.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zf.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://df.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eg.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://to.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mt.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vr.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mb.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rn.9csxet.cn

[P04] 求长度
来源：http://ui.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://db.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cm.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://js.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cj.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://wz.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://mh.shxzskj.cn

Ruby: x.length;  x.size
来源：http://pb.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ul.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://zy.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pg.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rq.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://az.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dg.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mq.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://js.huixinmuqiang.cn

Ruby: a == b
来源：http://kr.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ph.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://io.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vo.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://ff.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yo.hnjuh.cn

TS:   if (x == null) {}
来源：http://au.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lh.yuexingan06.cn

Go:   if x == nil {}
来源：http://xq.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bd.yuexingan06.cn

C#:   if (x is null) {}
来源：http://dp.shxzukj.cn

[P07] 防抖与节流
来源：http://ie.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dl.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://ns.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rs.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hy.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uh.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cp.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ci.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yh.hahajie.cn

[P08] 处理浮点精度问题
来源：http://gy.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fn.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xf.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fw.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ce.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yr.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mw.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://am.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gd.9csxet.cn

================================================================================
来源：http://ag.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jm.bookmarksfly.cn

================================================================================
来源：http://gf.nicolike.cn

[Q01] 创建表
来源：http://ay.521024.cn

CREATE TABLE users (
来源：http://ly.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yx.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://xt.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://bp.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ro.gzmigu.cn

);
来源：http://aa.hahajie.cn

[Q02] 创建带外键的表
来源：http://vu.yuexingan06.cn

CREATE TABLE orders (
来源：http://mn.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yq.nszjky.cn

user_id INT NOT NULL,
来源：http://lt.asd995.cn

amount DECIMAL(10, 2),
来源：http://mc.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gp.9csxet.cn

);
来源：http://js.bjjhwx.cn

[Q03] 增加列
来源：http://wu.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://en.521024.cn

[Q04] 修改列类型
来源：http://at.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yr.bjjhwx.cn

[Q05] 重命名列
来源：http://iz.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ct.nicolike.cn

[Q06] 删除列
来源：http://ss.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nf.9csxet.cn

[Q07] 删除表
来源：http://eb.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://pe.huanxung.cn

[Q08] 创建普通索引
来源：http://pt.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pu.colortex.cn

[Q09] 创建唯一索引
来源：http://uz.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pg.hnjuh.cn

[Q10] 插入单行
来源：http://sd.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hb.gzmigu.cn

[Q11] 一次插入多行
来源：http://cj.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lg.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://xh.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eg.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nv.asd995.cn

[Q13] 忽略重复插入
来源：http://yr.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mt.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://ma.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fk.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fz.nszjky.cn

[Q15] 查询全部
来源：http://he.lnxyls.cn

SELECT * FROM users;
来源：http://wx.gzmigu.cn

[Q16] 查询指定列
来源：http://fu.muxihuayi.cn

SELECT id, name FROM users;
来源：http://iq.nicolike.cn

[Q17] 条件查询
来源：http://yf.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rn.nszjky.cn

[Q18] 模糊匹配
来源：http://ye.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qb.colortex.cn

[Q19] 范围查询
来源：http://bz.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xj.yuntaijiaju.cn

[Q20] IN 列表
来源：http://bg.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ep.wgjwhj.cn

[Q21] 空值判断
来源：http://qp.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qu.chemitech.net.cn

[Q22] 排序
来源：http://jd.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dd.hahajie.cn

[Q23] 分页
来源：http://kl.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yq.szxytkj.cn

[Q24] 去重
来源：http://ws.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://dg.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://fy.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://je.asd995.cn

[Q26] 计数
来源：http://rw.521024.cn

SELECT COUNT(*) FROM users;
来源：http://lc.wgjwhj.cn

[Q27] 条件计数
来源：http://tz.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rz.shtwfgs.cn

[Q28] 求和与平均
来源：http://jb.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uw.szxytkj.cn

[Q29] 最大最小值
来源：http://st.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jv.szxytkj.cn

[Q30] 分组统计
来源：http://nj.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oj.nicolike.cn

[Q31] 分组后过滤
来源：http://wz.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://de.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://yp.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ij.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vm.huixiangedu.cn

[Q33] 多列分组
来源：http://vy.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hr.shxzskj.cn

[Q34] 每组取第一条
来源：http://hl.lnxyls.cn

SELECT * FROM (
来源：http://ed.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ej.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://gi.shxzukj.cn

[Q35] 内连接
来源：http://ra.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ah.chemitech.net.cn

[Q36] 左连接
来源：http://ns.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iv.lnxyls.cn

[Q37] 右连接
来源：http://jt.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nk.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lb.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rp.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://hr.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vf.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bw.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ak.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nu.hnjuh.cn

[Q41] 多表连接
来源：http://nr.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sr.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://an.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://jr.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://sx.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://pa.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yz.bjjhwx.cn

[Q43] 标量子查询
来源：http://bg.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qg.muxihuayi.cn

[Q44] IN 子查询
来源：http://th.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kd.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://ms.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sl.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qp.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nd.521024.cn

[Q47] 与平均值比较
来源：http://og.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vf.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://ot.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://on.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://rp.huanxung.cn

[Q49] 更新单行
来源：http://jj.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nu.jctech888.com.cn

[Q50] 批量更新
来源：http://em.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://js.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://ro.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fq.wgjwhj.cn

[Q52] 删除指定行
来源：http://ga.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://ax.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://cx.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nd.szxytkj.cn

[Q54] 清空表
来源：http://ao.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://us.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://gs.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ol.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://tl.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mr.shxzskj.cn

[Q57] 行号
来源：http://nw.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ua.9csxet.cn

[Q58] 累计求和
来源：http://lo.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jc.szsharing.cn

[Q59] 分组内累计
来源：http://ad.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cc.521024.cn

[Q60] 取上一行 / 下一行
来源：http://nd.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ii.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sq.lnxyls.cn

[Q61] 移动平均
来源：http://tn.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fd.asd995.cn

[Q62] 分组占比
来源：http://em.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sn.muxihuayi.cn

[Q63] 开启事务
来源：http://zg.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iy.panjiajie.cn

[Q64] 提交事务
来源：http://xq.hahajie.cn

COMMIT;
来源：http://by.colortex.cn

[Q65] 回滚事务
来源：http://lx.hnjuh.cn

ROLLBACK;
来源：http://uy.muxihuayi.cn

[Q66] 行锁查询
来源：http://il.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://an.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://qe.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qa.haigaiapp.cn

[Q68] 保存点
来源：http://kl.yuexingan06.cn

SAVEPOINT sp1;
来源：http://iv.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://mn.colortex.cn

[Q69] 查看执行计划
来源：http://nz.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ew.521024.cn

[Q70] 更新统计信息
来源：http://ur.nicolike.cn

ANALYZE TABLE users;
来源：http://gy.huixiangedu.cn

[Q71] 查看建表语句
来源：http://jc.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vt.huanxung.cn

[Q72] 查看索引
来源：http://xe.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://il.hahajie.cn

[Q73] 查看表状态
来源：http://cy.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jb.szxytkj.cn

[Q74] 强制使用索引
来源：http://dz.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ff.haigaiapp.cn

[Q75] 日期格式化
来源：http://we.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://my.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xr.bjjhwx.cn

[Q76] 按天统计
来源：http://vh.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jp.colortex.cn

[Q77] 时间加减
来源：http://ej.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ks.szsharing.cn

[Q78] 当前时间
来源：http://we.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dt.hnjuh.cn

[Q79] 字符串拼接
来源：http://qt.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xe.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://oh.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bp.panjiajie.cn

[Q81] 字符串替换
来源：http://ck.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mq.bjjhwx.cn


<!-- 参考信息 -->