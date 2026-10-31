代发 wailian999

================================================================================
来源：http://rp.muxihuayi.cn

O. 并发与异步
来源：http://km.521024.cn

================================================================================
来源：http://su.nszjky.cn

[O01] 启动一个线程
来源：http://fh.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zm.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qa.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hu.jctech888.com.cn

TS:   // 同 JS
来源：http://pa.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://bq.huixiangedu.cn

Go:   go f()
来源：http://pz.huanxung.cn

Ruby: Thread.new { f }
来源：http://ar.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://wb.nszjky.cn

[O02] 使用线程池
来源：http://sq.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sv.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vn.newstarts.cn

JS:   // worker_threads 线程池
来源：http://vw.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://mt.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zw.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hd.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hu.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ql.colortex.cn

[O03] 加锁保护共享数据
来源：http://ux.lnxyls.cn

Py:   with lock: shared += 1
来源：http://ju.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://dn.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sr.jianghongdianzi.cn

TS:   // 同 JS
来源：http://tf.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://kk.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aa.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jv.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://kd.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://gf.colortex.cn

Py:   async def f():⏎    await g()
来源：http://ke.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iq.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://ng.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mv.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lw.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cy.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ha.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://fz.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://tt.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://xi.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ka.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://bz.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://si.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dq.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sf.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://wl.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ib.hnjuh.cn

[O06] 使用进程池
来源：http://ra.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ov.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wb.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://nh.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://gh.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jj.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ax.muxihuayi.cn

Ruby: // fork 块
来源：http://en.bjjhwx.cn

C#:   Parallel.For
来源：http://kh.chemitech.net.cn

================================================================================
来源：http://wy.huixiangedu.cn

P. 常用工具函数
来源：http://il.bookmarksfly.cn

================================================================================
来源：http://sv.huixiangedu.cn

[P01] 生成 UUID
来源：http://wd.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://bc.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cu.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://vv.9csxet.cn

TS:   crypto.randomUUID()
来源：http://sq.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://bw.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://zu.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://dc.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://us.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://qx.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jc.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cd.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vq.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pw.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mv.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tp.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kr.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dh.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://qg.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://go.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pe.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xw.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nr.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ic.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ua.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://of.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qk.nicolike.cn

[P04] 求长度
来源：http://pk.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ln.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pt.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vy.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ko.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://jw.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://qd.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://ap.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lb.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://tu.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ui.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://my.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://se.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pj.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ne.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bp.nicolike.cn

Ruby: a == b
来源：http://mz.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qu.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xi.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jt.colortex.cn

PHP:  if (empty($x)) {}
来源：http://ts.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qd.shxzukj.cn

TS:   if (x == null) {}
来源：http://dx.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pk.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://sx.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pk.asd995.cn

C#:   if (x is null) {}
来源：http://ie.szsharing.cn

[P07] 防抖与节流
来源：http://pn.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ch.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://tv.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wn.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vt.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sq.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://za.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oi.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ae.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://jd.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://le.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hk.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rj.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ur.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ck.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bw.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dx.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fm.szsharing.cn

================================================================================
来源：http://po.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pl.gzmigu.cn

================================================================================
来源：http://hm.shxzukj.cn

[Q01] 创建表
来源：http://qm.yuntaijiaju.cn

CREATE TABLE users (
来源：http://xn.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lp.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://gt.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://eo.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zo.newstarts.cn

);
来源：http://sd.nszjky.cn

[Q02] 创建带外键的表
来源：http://dh.bookmarksfly.cn

CREATE TABLE orders (
来源：http://wd.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zf.nszjky.cn

user_id INT NOT NULL,
来源：http://ir.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://fe.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qt.jianghongdianzi.cn

);
来源：http://ie.bjjhwx.cn

[Q03] 增加列
来源：http://vw.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cj.newstarts.cn

[Q04] 修改列类型
来源：http://uy.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kc.shtwfgs.cn

[Q05] 重命名列
来源：http://xm.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eo.nicolike.cn

[Q06] 删除列
来源：http://md.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kh.gzmigu.cn

[Q07] 删除表
来源：http://ds.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://rz.jctech888.com.cn

[Q08] 创建普通索引
来源：http://xh.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ve.9csxet.cn

[Q09] 创建唯一索引
来源：http://nq.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ii.9csxet.cn

[Q10] 插入单行
来源：http://il.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wl.bjjhwx.cn

[Q11] 一次插入多行
来源：http://nb.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bn.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://dk.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://em.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vw.9csxet.cn

[Q13] 忽略重复插入
来源：http://ug.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vb.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://ps.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://et.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hv.asd995.cn

[Q15] 查询全部
来源：http://jf.shtwfgs.cn

SELECT * FROM users;
来源：http://rt.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://cw.bjjhwx.cn

SELECT id, name FROM users;
来源：http://rd.bookmarksfly.cn

[Q17] 条件查询
来源：http://ue.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://di.asd995.cn

[Q18] 模糊匹配
来源：http://gj.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ex.newstarts.cn

[Q19] 范围查询
来源：http://ru.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rt.bookmarksfly.cn

[Q20] IN 列表
来源：http://de.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jt.hahajie.cn

[Q21] 空值判断
来源：http://ep.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wr.jianghongdianzi.cn

[Q22] 排序
来源：http://gd.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://se.jianghongdianzi.cn

[Q23] 分页
来源：http://ur.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jd.huanxung.cn

[Q24] 去重
来源：http://lw.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://xv.9csxet.cn

[Q25] 只取前 N 条
来源：http://ma.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kb.shxzskj.cn

[Q26] 计数
来源：http://sd.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://xm.9csxet.cn

[Q27] 条件计数
来源：http://pk.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tq.jctech888.com.cn

[Q28] 求和与平均
来源：http://we.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gp.shtwfgs.cn

[Q29] 最大最小值
来源：http://wj.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cr.panjiajie.cn

[Q30] 分组统计
来源：http://lf.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vb.shxzukj.cn

[Q31] 分组后过滤
来源：http://wn.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ww.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://it.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wk.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kj.huixiangedu.cn

[Q33] 多列分组
来源：http://fb.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aq.521024.cn

[Q34] 每组取第一条
来源：http://xx.shxzskj.cn

SELECT * FROM (
来源：http://pn.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qr.newstarts.cn

) t WHERE rn = 1;
来源：http://yq.lnxyls.cn

[Q35] 内连接
来源：http://cd.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wm.chemitech.net.cn

[Q36] 左连接
来源：http://dy.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tf.521024.cn

[Q37] 右连接
来源：http://bh.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vv.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qq.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://in.asd995.cn

[Q39] 自连接（查上下级）
来源：http://of.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fk.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dq.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bp.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vp.panjiajie.cn

[Q41] 多表连接
来源：http://sy.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qc.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://yr.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://ji.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://ae.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://xf.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yq.hahajie.cn

[Q43] 标量子查询
来源：http://cl.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://al.hnjuh.cn

[Q44] IN 子查询
来源：http://uy.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lx.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://md.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hb.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pm.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zo.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://xx.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lr.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://cp.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ck.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://oi.colortex.cn

[Q49] 更新单行
来源：http://ez.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ss.szsharing.cn

[Q50] 批量更新
来源：http://lr.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://po.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://eg.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://br.huanxung.cn

[Q52] 删除指定行
来源：http://ph.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://to.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://la.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jn.shxzukj.cn

[Q54] 清空表
来源：http://zb.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://if.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://nn.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ft.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://ua.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ge.colortex.cn

[Q57] 行号
来源：http://rv.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jd.hnjuh.cn

[Q58] 累计求和
来源：http://jf.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pm.hahajie.cn

[Q59] 分组内累计
来源：http://fh.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://du.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://bm.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sr.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ig.newstarts.cn

[Q61] 移动平均
来源：http://ou.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vl.shxzukj.cn

[Q62] 分组占比
来源：http://dr.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ct.huanxung.cn

[Q63] 开启事务
来源：http://sr.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mv.shtwfgs.cn

[Q64] 提交事务
来源：http://sa.muxihuayi.cn

COMMIT;
来源：http://bc.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://ny.huanxung.cn

ROLLBACK;
来源：http://jw.jctech888.com.cn

[Q66] 行锁查询
来源：http://gb.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lf.huanxung.cn

[Q67] 设置隔离级别
来源：http://yr.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://du.colortex.cn

[Q68] 保存点
来源：http://pr.nicolike.cn

SAVEPOINT sp1;
来源：http://wv.hahajie.cn

ROLLBACK TO sp1;
来源：http://uv.gzmigu.cn

[Q69] 查看执行计划
来源：http://nu.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nb.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://dv.muxihuayi.cn

ANALYZE TABLE users;
来源：http://kd.szsharing.cn

[Q71] 查看建表语句
来源：http://qy.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tz.yuntaijiaju.cn

[Q72] 查看索引
来源：http://mg.newstarts.cn


<!-- 参考信息 -->