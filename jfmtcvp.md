代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://we.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ge.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fn.muxihuayi.cn

TS:   // 同 JS
来源：http://eu.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://aj.9csxet.cn

Go:   go f()
来源：http://wk.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://aw.9csxet.cn

C#:   Task.Run(() => F());
来源：http://gd.wgjwhj.cn

[O02] 使用线程池
来源：http://gr.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ul.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dp.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://xo.newstarts.cn

TS:   // worker_threads 线程池
来源：http://hv.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tg.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mw.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aj.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eg.colortex.cn

[O03] 加锁保护共享数据
来源：http://vw.521024.cn

Py:   with lock: shared += 1
来源：http://yv.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://hs.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://us.chemitech.net.cn

TS:   // 同 JS
来源：http://nl.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://td.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tm.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://au.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://gk.newstarts.cn

[O04] 定义异步函数并等待
来源：http://po.colortex.cn

Py:   async def f():⏎    await g()
来源：http://lz.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qj.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://fv.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gm.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kg.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hg.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lg.colortex.cn

C#:   async Task F() { await G(); }
来源：http://ok.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://xy.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://he.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ao.asd995.cn

JS:   await Promise.all(tasks)
来源：http://oh.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://xs.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gc.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ug.521024.cn

Ruby: threads.map(&:join)
来源：http://vx.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ry.9csxet.cn

[O06] 使用进程池
来源：http://mp.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ts.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ez.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://xx.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://xx.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xb.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xl.jctech888.com.cn

Ruby: // fork 块
来源：http://ln.huixiangedu.cn

C#:   Parallel.For
来源：http://gx.chemitech.net.cn

================================================================================
来源：http://rm.shxzskj.cn

P. 常用工具函数
来源：http://sb.bookmarksfly.cn

================================================================================
来源：http://lh.haigaiapp.cn

[P01] 生成 UUID
来源：http://ev.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://ex.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oy.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://od.nszjky.cn

TS:   crypto.randomUUID()
来源：http://hc.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://mp.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://qy.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://yb.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://wz.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://ow.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qt.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://se.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gd.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qb.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ic.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cb.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rr.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://km.shxzukj.cn

[P03] 生成短随机字符串
来源：http://yy.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uv.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://es.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fm.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://db.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vs.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ih.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://to.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mu.shxzskj.cn

[P04] 求长度
来源：http://bz.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ki.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nk.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mv.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xm.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://sb.hahajie.cn

Go:   len(arr);  len(m)
来源：http://to.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://dn.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xd.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://mr.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lu.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vd.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://li.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lp.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sj.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://il.chemitech.net.cn

Ruby: a == b
来源：http://fq.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kp.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qj.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lp.521024.cn

PHP:  if (empty($x)) {}
来源：http://le.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://he.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://ho.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ia.hnjuh.cn

Go:   if x == nil {}
来源：http://hy.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hn.asd995.cn

C#:   if (x is null) {}
来源：http://st.hahajie.cn

[P07] 防抖与节流
来源：http://fq.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ug.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://ij.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://la.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nz.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://li.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dd.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iv.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hh.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://zf.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yd.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qr.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zv.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ck.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nw.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uk.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ky.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nd.szsharing.cn

================================================================================
来源：http://lf.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pi.huanxung.cn

================================================================================
来源：http://cv.asd995.cn

[Q01] 创建表
来源：http://wm.nszjky.cn

CREATE TABLE users (
来源：http://fw.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yj.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://gl.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://jy.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ok.wgjwhj.cn

);
来源：http://ax.huanxung.cn

[Q02] 创建带外键的表
来源：http://nh.wgjwhj.cn

CREATE TABLE orders (
来源：http://ko.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wo.jctech888.com.cn

user_id INT NOT NULL,
来源：http://iy.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://am.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zb.yuntaijiaju.cn

);
来源：http://sw.szxytkj.cn

[Q03] 增加列
来源：http://ca.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://on.hahajie.cn

[Q04] 修改列类型
来源：http://lz.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oh.bookmarksfly.cn

[Q05] 重命名列
来源：http://vr.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://av.521024.cn

[Q06] 删除列
来源：http://ve.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kx.9csxet.cn

[Q07] 删除表
来源：http://jy.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://wc.chemitech.net.cn

[Q08] 创建普通索引
来源：http://ri.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://te.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://uz.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vd.szsharing.cn

[Q10] 插入单行
来源：http://sp.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yp.newstarts.cn

[Q11] 一次插入多行
来源：http://zd.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iv.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://kn.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ai.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lw.newstarts.cn

[Q13] 忽略重复插入
来源：http://uu.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ms.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://fs.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fp.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kl.521024.cn

[Q15] 查询全部
来源：http://eo.haigaiapp.cn

SELECT * FROM users;
来源：http://ae.521024.cn

[Q16] 查询指定列
来源：http://vz.chemitech.net.cn

SELECT id, name FROM users;
来源：http://oy.jianghongdianzi.cn

[Q17] 条件查询
来源：http://pb.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://th.asd995.cn

[Q18] 模糊匹配
来源：http://cp.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qr.huixinmuqiang.cn

[Q19] 范围查询
来源：http://ef.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bp.huixinmuqiang.cn

[Q20] IN 列表
来源：http://kf.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yy.bookmarksfly.cn

[Q21] 空值判断
来源：http://el.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vb.wgjwhj.cn

[Q22] 排序
来源：http://ko.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tb.shxzskj.cn

[Q23] 分页
来源：http://ce.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vr.shxzskj.cn

[Q24] 去重
来源：http://xf.521024.cn

SELECT DISTINCT city FROM users;
来源：http://pj.colortex.cn

[Q25] 只取前 N 条
来源：http://dn.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://as.nicolike.cn

[Q26] 计数
来源：http://bd.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://eu.9csxet.cn

[Q27] 条件计数
来源：http://pi.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cb.bjjhwx.cn

[Q28] 求和与平均
来源：http://zg.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zh.hahajie.cn

[Q29] 最大最小值
来源：http://gk.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iu.haigaiapp.cn

[Q30] 分组统计
来源：http://mq.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vs.wgjwhj.cn

[Q31] 分组后过滤
来源：http://po.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wa.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://xh.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ag.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jh.muxihuayi.cn

[Q33] 多列分组
来源：http://zz.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zm.huixiangedu.cn

[Q34] 每组取第一条
来源：http://hf.asd995.cn

SELECT * FROM (
来源：http://nj.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jc.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://yf.hnjuh.cn

[Q35] 内连接
来源：http://yf.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ls.hnjuh.cn

[Q36] 左连接
来源：http://no.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iv.szxytkj.cn

[Q37] 右连接
来源：http://jl.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cz.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mo.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tt.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://wr.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://si.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zk.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qh.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://td.huixinmuqiang.cn

[Q41] 多表连接
来源：http://qq.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wq.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://jc.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://zx.colortex.cn

[Q42] 连接条件附加过滤
来源：http://pv.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://oh.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ja.asd995.cn

[Q43] 标量子查询
来源：http://nk.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rx.haigaiapp.cn

[Q44] IN 子查询
来源：http://hc.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://la.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://ze.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xx.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nn.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vr.chemitech.net.cn

[Q47] 与平均值比较
来源：http://qg.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tc.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://rs.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nn.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://zf.newstarts.cn

[Q49] 更新单行
来源：http://kg.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ep.szsharing.cn

[Q50] 批量更新
来源：http://tf.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zp.asd995.cn

[Q51] 用子查询更新
来源：http://dj.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://es.panjiajie.cn

[Q52] 删除指定行
来源：http://un.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://ao.szsharing.cn

[Q53] 按条件删除
来源：http://ws.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jk.haigaiapp.cn

[Q54] 清空表
来源：http://wf.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://ab.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://gq.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fv.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ke.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lh.yuntaijiaju.cn

[Q57] 行号
来源：http://ws.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ii.bookmarksfly.cn

[Q58] 累计求和
来源：http://hh.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lx.shtwfgs.cn

[Q59] 分组内累计
来源：http://xl.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dk.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://fj.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ff.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ys.muxihuayi.cn

[Q61] 移动平均
来源：http://io.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lr.panjiajie.cn

[Q62] 分组占比
来源：http://xx.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cq.szsharing.cn

[Q63] 开启事务
来源：http://vx.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wh.shxzskj.cn

[Q64] 提交事务
来源：http://fr.hahajie.cn

COMMIT;
来源：http://ua.chemitech.net.cn

[Q65] 回滚事务
来源：http://nd.haigaiapp.cn

ROLLBACK;
来源：http://hm.wgjwhj.cn

[Q66] 行锁查询
来源：http://rq.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vj.asd995.cn

[Q67] 设置隔离级别
来源：http://jc.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fy.shtwfgs.cn

[Q68] 保存点
来源：http://hr.jctech888.com.cn

SAVEPOINT sp1;
来源：http://aa.huanxung.cn

ROLLBACK TO sp1;
来源：http://ie.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://zu.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zr.bjjhwx.cn

[Q70] 更新统计信息
来源：http://zh.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://vt.newstarts.cn

[Q71] 查看建表语句
来源：http://zk.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ie.jianghongdianzi.cn

[Q72] 查看索引
来源：http://az.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://nq.szxytkj.cn

[Q73] 查看表状态
来源：http://es.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xq.521024.cn

[Q74] 强制使用索引
来源：http://ii.szxytkj.cn


<!-- 参考信息 -->