代发 wailian999

TS:   // worker_threads 线程池
来源：http://ro.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tv.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mt.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yd.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mo.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://ls.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://xo.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://rq.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://if.huixiangedu.cn

TS:   // 同 JS
来源：http://ba.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://ly.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lh.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lu.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://rt.colortex.cn

[O04] 定义异步函数并等待
来源：http://mz.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://wt.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rd.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://jw.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uc.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mg.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zl.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vz.asd995.cn

C#:   async Task F() { await G(); }
来源：http://rm.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://pf.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://ml.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gz.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://yk.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://cq.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://at.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xw.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://tf.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iw.hnjuh.cn

[O06] 使用进程池
来源：http://nk.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qr.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xk.521024.cn

JS:   // child_process / cluster 模块
来源：http://si.colortex.cn

TS:   // child_process / cluster 模块
来源：http://ez.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xq.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wz.yuntaijiaju.cn

Ruby: // fork 块
来源：http://si.bookmarksfly.cn

C#:   Parallel.For
来源：http://gb.nszjky.cn

================================================================================
来源：http://yk.yuexingan06.cn

P. 常用工具函数
来源：http://ip.hahajie.cn

================================================================================
来源：http://gy.jctech888.com.cn

[P01] 生成 UUID
来源：http://zq.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://lb.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sg.huanxung.cn

JS:   crypto.randomUUID()
来源：http://gu.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://am.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://aq.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://qm.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://sy.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://kq.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://nw.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ll.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ci.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uk.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://te.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vs.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://la.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cf.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hb.hnjuh.cn

[P03] 生成短随机字符串
来源：http://zj.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ri.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tw.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kw.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fe.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zm.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ec.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ni.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fw.chemitech.net.cn

[P04] 求长度
来源：http://bj.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vv.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ku.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wb.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ui.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://jb.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://wa.9csxet.cn

Ruby: x.length;  x.size
来源：http://ra.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vx.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://uf.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://so.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lu.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://za.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://co.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://he.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wz.bookmarksfly.cn

Ruby: a == b
来源：http://mf.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uc.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uc.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tc.colortex.cn

PHP:  if (empty($x)) {}
来源：http://rz.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mf.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://in.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hw.9csxet.cn

Go:   if x == nil {}
来源：http://wg.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cg.shxzukj.cn

C#:   if (x is null) {}
来源：http://ph.panjiajie.cn

[P07] 防抖与节流
来源：http://wt.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pn.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://ms.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vh.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ie.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ie.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wh.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fk.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jj.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://yg.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qi.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yj.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wl.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xt.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vu.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lc.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ke.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ew.huixiangedu.cn

================================================================================
来源：http://oo.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://if.haigaiapp.cn

================================================================================
来源：http://tr.nszjky.cn

[Q01] 创建表
来源：http://ku.9csxet.cn

CREATE TABLE users (
来源：http://jw.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ma.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://qm.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://gq.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zb.shxzukj.cn

);
来源：http://bu.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://ik.hahajie.cn

CREATE TABLE orders (
来源：http://ry.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dy.muxihuayi.cn

user_id INT NOT NULL,
来源：http://vk.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://hr.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pa.huixiangedu.cn

);
来源：http://gh.panjiajie.cn

[Q03] 增加列
来源：http://fl.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vv.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://xt.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qt.lnxyls.cn

[Q05] 重命名列
来源：http://yn.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://es.bjjhwx.cn

[Q06] 删除列
来源：http://lr.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://us.huixinmuqiang.cn

[Q07] 删除表
来源：http://fv.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://xl.muxihuayi.cn

[Q08] 创建普通索引
来源：http://ue.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yf.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://es.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jc.bjjhwx.cn

[Q10] 插入单行
来源：http://ns.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://me.nszjky.cn

[Q11] 一次插入多行
来源：http://xx.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ol.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://um.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yv.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vf.asd995.cn

[Q13] 忽略重复插入
来源：http://wn.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xk.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://rw.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nz.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oc.yuexingan06.cn

[Q15] 查询全部
来源：http://yj.yuntaijiaju.cn

SELECT * FROM users;
来源：http://ab.nszjky.cn

[Q16] 查询指定列
来源：http://au.jctech888.com.cn

SELECT id, name FROM users;
来源：http://dq.shxzukj.cn

[Q17] 条件查询
来源：http://ag.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ad.chemitech.net.cn

[Q18] 模糊匹配
来源：http://xo.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oi.huanxung.cn

[Q19] 范围查询
来源：http://lo.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yf.jctech888.com.cn

[Q20] IN 列表
来源：http://if.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fp.szxytkj.cn

[Q21] 空值判断
来源：http://ec.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hq.muxihuayi.cn

[Q22] 排序
来源：http://rr.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sk.9csxet.cn

[Q23] 分页
来源：http://iw.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ih.bjjhwx.cn

[Q24] 去重
来源：http://dr.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://it.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://mz.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nx.szxytkj.cn

[Q26] 计数
来源：http://gb.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://eo.521024.cn

[Q27] 条件计数
来源：http://nl.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://px.chemitech.net.cn

[Q28] 求和与平均
来源：http://jo.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ln.huixiangedu.cn

[Q29] 最大最小值
来源：http://iw.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zs.bjjhwx.cn

[Q30] 分组统计
来源：http://ac.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jx.huanxung.cn

[Q31] 分组后过滤
来源：http://hk.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gi.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://zl.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ec.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aq.nszjky.cn

[Q33] 多列分组
来源：http://fp.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://do.huanxung.cn

[Q34] 每组取第一条
来源：http://ou.muxihuayi.cn

SELECT * FROM (
来源：http://uh.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ii.jctech888.com.cn

) t WHERE rn = 1;
来源：http://cr.521024.cn

[Q35] 内连接
来源：http://xg.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ye.huixinmuqiang.cn

[Q36] 左连接
来源：http://xh.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fx.szxytkj.cn

[Q37] 右连接
来源：http://ur.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vq.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zo.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gl.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://ti.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wq.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ja.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://je.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ez.hahajie.cn

[Q41] 多表连接
来源：http://bu.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dp.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://oz.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://cu.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://mn.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://hy.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qg.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://xt.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sx.haigaiapp.cn

[Q44] IN 子查询
来源：http://eq.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ko.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://ym.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ng.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ed.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ci.wgjwhj.cn

[Q47] 与平均值比较
来源：http://pt.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sw.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://cg.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xn.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://ag.haigaiapp.cn

[Q49] 更新单行
来源：http://hc.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ev.muxihuayi.cn

[Q50] 批量更新
来源：http://dh.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aj.huixiangedu.cn

[Q51] 用子查询更新
来源：http://yy.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jo.wgjwhj.cn

[Q52] 删除指定行
来源：http://cy.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://mr.muxihuayi.cn

[Q53] 按条件删除
来源：http://wk.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yw.szxytkj.cn

[Q54] 清空表
来源：http://ej.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://yx.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://kt.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zf.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://qw.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nz.huixiangedu.cn

[Q57] 行号
来源：http://ed.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jm.muxihuayi.cn

[Q58] 累计求和
来源：http://us.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lf.gzmigu.cn

[Q59] 分组内累计
来源：http://xy.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://si.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://fm.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gy.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ip.yuntaijiaju.cn

[Q61] 移动平均
来源：http://uo.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ts.521024.cn

[Q62] 分组占比
来源：http://ui.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wh.huanxung.cn

[Q63] 开启事务
来源：http://gy.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hc.newstarts.cn

[Q64] 提交事务
来源：http://wh.haigaiapp.cn

COMMIT;
来源：http://ug.muxihuayi.cn

[Q65] 回滚事务
来源：http://vl.huixinmuqiang.cn

ROLLBACK;
来源：http://kw.bjjhwx.cn

[Q66] 行锁查询
来源：http://ov.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eo.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://wh.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rj.huixiangedu.cn

[Q68] 保存点
来源：http://gw.521024.cn

SAVEPOINT sp1;
来源：http://mn.hahajie.cn

ROLLBACK TO sp1;
来源：http://wt.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://tk.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://so.haigaiapp.cn

[Q70] 更新统计信息
来源：http://kt.yuexingan06.cn

ANALYZE TABLE users;
来源：http://am.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://uk.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fq.lnxyls.cn

[Q72] 查看索引
来源：http://pz.hahajie.cn

SHOW INDEX FROM users;
来源：http://ac.shxzskj.cn

[Q73] 查看表状态
来源：http://uv.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://no.colortex.cn

[Q74] 强制使用索引
来源：http://vu.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ep.9csxet.cn

[Q75] 日期格式化
来源：http://sb.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hr.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mj.bjjhwx.cn

[Q76] 按天统计
来源：http://za.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://po.huixinmuqiang.cn

[Q77] 时间加减
来源：http://kc.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nb.haigaiapp.cn

[Q78] 当前时间
来源：http://ls.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qh.hnjuh.cn

[Q79] 字符串拼接
来源：http://tb.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oo.muxihuayi.cn


<!-- 参考信息 -->