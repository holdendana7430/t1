代发 wailian999

================================================================================
来源：http://hu.asd995.cn

O. 并发与异步
来源：http://zd.huanxung.cn

================================================================================
来源：http://un.colortex.cn

[O01] 启动一个线程
来源：http://ca.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kl.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fl.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qd.gzmigu.cn

TS:   // 同 JS
来源：http://kx.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://or.jianghongdianzi.cn

Go:   go f()
来源：http://mu.colortex.cn

Ruby: Thread.new { f }
来源：http://nj.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://yc.9csxet.cn

[O02] 使用线程池
来源：http://xn.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mj.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gs.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://qp.nszjky.cn

TS:   // worker_threads 线程池
来源：http://rv.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vp.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oy.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qw.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uz.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://wa.szxytkj.cn

Py:   with lock: shared += 1
来源：http://yh.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://jk.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ew.hahajie.cn

TS:   // 同 JS
来源：http://ge.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://el.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xu.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ov.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://dt.521024.cn

[O04] 定义异步函数并等待
来源：http://qs.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://wd.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gb.huanxung.cn

JS:   async function f() { await g(); }
来源：http://ce.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ob.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mb.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pb.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kr.colortex.cn

C#:   async Task F() { await G(); }
来源：http://cl.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://kc.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://lu.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tm.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://qx.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://iq.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iu.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wq.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://wj.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jc.hnjuh.cn

[O06] 使用进程池
来源：http://go.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uq.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zo.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://db.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://jz.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ea.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vx.szsharing.cn

Ruby: // fork 块
来源：http://jg.newstarts.cn

C#:   Parallel.For
来源：http://mg.szsharing.cn

================================================================================
来源：http://ef.yuexingan06.cn

P. 常用工具函数
来源：http://tn.yuexingan06.cn

================================================================================
来源：http://zm.shxzukj.cn

[P01] 生成 UUID
来源：http://ha.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://km.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bb.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://dj.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://nl.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://gj.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://vj.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://pv.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://vv.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://jd.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ef.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qd.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dw.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fe.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ow.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fv.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dv.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ai.lnxyls.cn

[P03] 生成短随机字符串
来源：http://qu.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ld.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xw.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bx.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wo.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xu.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sc.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ab.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dr.shtwfgs.cn

[P04] 求长度
来源：http://cm.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fo.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qk.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nd.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jw.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://tn.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://ha.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://gz.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ou.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://ap.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://no.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ta.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uc.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zg.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vx.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ox.shxzskj.cn

Ruby: a == b
来源：http://sx.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sc.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://og.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://se.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://sl.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jp.nszjky.cn

TS:   if (x == null) {}
来源：http://ui.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bj.9csxet.cn

Go:   if x == nil {}
来源：http://pv.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ny.haigaiapp.cn

C#:   if (x is null) {}
来源：http://vc.hahajie.cn

[P07] 防抖与节流
来源：http://pz.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gv.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://es.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sn.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vw.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lb.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mh.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uk.huanxung.cn

[P08] 处理浮点精度问题
来源：http://cl.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kn.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fj.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mg.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ig.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gv.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gd.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://se.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ko.huixiangedu.cn

================================================================================
来源：http://dw.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gk.newstarts.cn

================================================================================
来源：http://cy.huixiangedu.cn

[Q01] 创建表
来源：http://vo.bjjhwx.cn

CREATE TABLE users (
来源：http://yv.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jr.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ap.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://mz.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eg.huanxung.cn

);
来源：http://pb.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://oz.9csxet.cn

CREATE TABLE orders (
来源：http://hx.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zq.colortex.cn

user_id INT NOT NULL,
来源：http://yy.hahajie.cn

amount DECIMAL(10, 2),
来源：http://yd.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mj.szsharing.cn

);
来源：http://ah.521024.cn

[Q03] 增加列
来源：http://aj.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cn.asd995.cn

[Q04] 修改列类型
来源：http://cd.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ho.nszjky.cn

[Q05] 重命名列
来源：http://sw.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ge.shtwfgs.cn

[Q06] 删除列
来源：http://ph.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uj.jianghongdianzi.cn

[Q07] 删除表
来源：http://ka.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://yk.newstarts.cn

[Q08] 创建普通索引
来源：http://ft.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nj.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://ev.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kk.huixiangedu.cn

[Q10] 插入单行
来源：http://as.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oj.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://mv.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bv.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://fz.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nm.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jj.nszjky.cn

[Q13] 忽略重复插入
来源：http://bf.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://si.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://mr.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qc.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cu.yuntaijiaju.cn

[Q15] 查询全部
来源：http://zy.huanxung.cn

SELECT * FROM users;
来源：http://rr.yuexingan06.cn

[Q16] 查询指定列
来源：http://jn.bjjhwx.cn

SELECT id, name FROM users;
来源：http://ae.hahajie.cn

[Q17] 条件查询
来源：http://ga.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jh.haigaiapp.cn

[Q18] 模糊匹配
来源：http://bv.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bh.chemitech.net.cn

[Q19] 范围查询
来源：http://py.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gf.bjjhwx.cn

[Q20] IN 列表
来源：http://eq.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qy.huixiangedu.cn

[Q21] 空值判断
来源：http://yw.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gh.9csxet.cn

[Q22] 排序
来源：http://pc.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rl.szsharing.cn

[Q23] 分页
来源：http://ko.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yf.huanxung.cn

[Q24] 去重
来源：http://gz.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://jl.szxytkj.cn

[Q25] 只取前 N 条
来源：http://mh.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://co.bjjhwx.cn

[Q26] 计数
来源：http://kr.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://oa.colortex.cn

[Q27] 条件计数
来源：http://og.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zd.wgjwhj.cn

[Q28] 求和与平均
来源：http://te.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://de.gzmigu.cn

[Q29] 最大最小值
来源：http://lj.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://af.szsharing.cn

[Q30] 分组统计
来源：http://ln.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ci.shxzskj.cn

[Q31] 分组后过滤
来源：http://xe.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lm.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://pn.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qz.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://df.9csxet.cn

[Q33] 多列分组
来源：http://vt.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jk.panjiajie.cn

[Q34] 每组取第一条
来源：http://gu.szsharing.cn

SELECT * FROM (
来源：http://tu.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bv.nicolike.cn

) t WHERE rn = 1;
来源：http://yi.yuntaijiaju.cn

[Q35] 内连接
来源：http://ph.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fq.gzmigu.cn

[Q36] 左连接
来源：http://oi.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ch.newstarts.cn

[Q37] 右连接
来源：http://rc.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gl.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vq.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tq.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://oh.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kd.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aw.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ew.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wf.huixiangedu.cn

[Q41] 多表连接
来源：http://js.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ps.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://wn.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vw.colortex.cn

[Q42] 连接条件附加过滤
来源：http://tc.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://rn.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mc.shtwfgs.cn

[Q43] 标量子查询
来源：http://io.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cq.gzmigu.cn

[Q44] IN 子查询
来源：http://ji.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vw.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://zv.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ae.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wu.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://du.jctech888.com.cn

[Q47] 与平均值比较
来源：http://hw.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://as.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://gp.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pn.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://cl.muxihuayi.cn

[Q49] 更新单行
来源：http://mk.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hy.huixinmuqiang.cn

[Q50] 批量更新
来源：http://db.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sz.chemitech.net.cn

[Q51] 用子查询更新
来源：http://cy.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ny.9csxet.cn

[Q52] 删除指定行
来源：http://ng.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://zx.jctech888.com.cn

[Q53] 按条件删除
来源：http://qd.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iq.nicolike.cn

[Q54] 清空表
来源：http://uv.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://ep.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://dt.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pk.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://wz.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ix.hnjuh.cn

[Q57] 行号
来源：http://vr.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://io.asd995.cn

[Q58] 累计求和
来源：http://oi.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ci.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://fi.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yr.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://js.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uk.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lv.hnjuh.cn

[Q61] 移动平均
来源：http://hs.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ry.szsharing.cn

[Q62] 分组占比
来源：http://zi.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yf.521024.cn

[Q63] 开启事务
来源：http://xe.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wc.hahajie.cn

[Q64] 提交事务
来源：http://rk.asd995.cn

COMMIT;
来源：http://zo.jctech888.com.cn

[Q65] 回滚事务
来源：http://iz.yuntaijiaju.cn

ROLLBACK;
来源：http://yz.shxzskj.cn

[Q66] 行锁查询
来源：http://tk.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://if.nszjky.cn

[Q67] 设置隔离级别
来源：http://rq.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ej.nszjky.cn

[Q68] 保存点
来源：http://hc.shxzukj.cn

SAVEPOINT sp1;
来源：http://en.szsharing.cn

ROLLBACK TO sp1;
来源：http://up.muxihuayi.cn

[Q69] 查看执行计划
来源：http://gg.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ht.szxytkj.cn

[Q70] 更新统计信息
来源：http://bx.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://dy.shxzukj.cn

[Q71] 查看建表语句
来源：http://bk.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vi.panjiajie.cn

[Q72] 查看索引
来源：http://gh.colortex.cn


<!-- 参考信息 -->