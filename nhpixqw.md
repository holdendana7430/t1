代发 wailian999

================================================================================
来源：http://hr.huixinmuqiang.cn

O. 并发与异步
来源：http://zj.nszjky.cn

================================================================================
来源：http://ie.shxzukj.cn

[O01] 启动一个线程
来源：http://le.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://km.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gu.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://te.shxzskj.cn

TS:   // 同 JS
来源：http://so.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://hf.huixinmuqiang.cn

Go:   go f()
来源：http://nq.gzmigu.cn

Ruby: Thread.new { f }
来源：http://jl.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://yh.521024.cn

[O02] 使用线程池
来源：http://di.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yg.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hb.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://xg.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://ec.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://be.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dx.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jd.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mn.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://yu.huanxung.cn

Py:   with lock: shared += 1
来源：http://it.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://sm.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xt.nszjky.cn

TS:   // 同 JS
来源：http://zy.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://hl.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wy.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rm.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://vh.asd995.cn

[O04] 定义异步函数并等待
来源：http://nl.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://qg.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hq.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://qb.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iv.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qr.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://in.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oe.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://xm.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://sn.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://fo.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oc.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://ks.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://pq.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lb.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fa.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://sz.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ne.hnjuh.cn

[O06] 使用进程池
来源：http://iy.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ok.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://em.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://ie.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://yz.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dn.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gx.nicolike.cn

Ruby: // fork 块
来源：http://cn.asd995.cn

C#:   Parallel.For
来源：http://bu.haigaiapp.cn

================================================================================
来源：http://ok.shtwfgs.cn

P. 常用工具函数
来源：http://eo.shtwfgs.cn

================================================================================
来源：http://mn.hnjuh.cn

[P01] 生成 UUID
来源：http://es.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://gq.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://et.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://bf.nicolike.cn

TS:   crypto.randomUUID()
来源：http://nb.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://ak.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://qs.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://sn.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://oi.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://to.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ry.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://in.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ng.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oz.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ef.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zn.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qk.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kq.hnjuh.cn

[P03] 生成短随机字符串
来源：http://ti.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mf.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ig.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mr.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xe.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qo.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cx.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ox.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://km.yuntaijiaju.cn

[P04] 求长度
来源：http://ge.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aw.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ai.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://er.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ly.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://al.asd995.cn

Go:   len(arr);  len(m)
来源：http://le.asd995.cn

Ruby: x.length;  x.size
来源：http://uz.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lq.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://td.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ho.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xk.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://md.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uc.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rw.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ti.hahajie.cn

Ruby: a == b
来源：http://xo.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rt.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ci.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sn.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://zk.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fc.szsharing.cn

TS:   if (x == null) {}
来源：http://qc.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rm.gzmigu.cn

Go:   if x == nil {}
来源：http://cn.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bo.shtwfgs.cn

C#:   if (x is null) {}
来源：http://kw.bjjhwx.cn

[P07] 防抖与节流
来源：http://qu.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wi.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://vq.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://om.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qv.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://il.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uk.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nj.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nh.szsharing.cn

[P08] 处理浮点精度问题
来源：http://rs.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ti.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cg.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hn.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://px.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xp.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fi.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ok.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jc.asd995.cn

================================================================================
来源：http://te.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ck.jctech888.com.cn

================================================================================
来源：http://tk.shxzskj.cn

[Q01] 创建表
来源：http://bs.asd995.cn

CREATE TABLE users (
来源：http://wy.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tr.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://uy.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://ss.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xe.shxzskj.cn

);
来源：http://xb.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://jy.huixiangedu.cn

CREATE TABLE orders (
来源：http://th.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mg.panjiajie.cn

user_id INT NOT NULL,
来源：http://lj.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://ls.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://to.panjiajie.cn

);
来源：http://ij.nszjky.cn

[Q03] 增加列
来源：http://zm.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rw.shxzukj.cn

[Q04] 修改列类型
来源：http://pu.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zs.yuntaijiaju.cn

[Q05] 重命名列
来源：http://kf.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://io.huixiangedu.cn

[Q06] 删除列
来源：http://pz.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tt.shtwfgs.cn

[Q07] 删除表
来源：http://ru.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://rz.szxytkj.cn

[Q08] 创建普通索引
来源：http://er.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zg.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://gi.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yb.yuntaijiaju.cn

[Q10] 插入单行
来源：http://tv.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ja.gzmigu.cn

[Q11] 一次插入多行
来源：http://wg.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pm.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://rb.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://et.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rt.colortex.cn

[Q13] 忽略重复插入
来源：http://gu.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ss.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://nt.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://is.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fr.9csxet.cn

[Q15] 查询全部
来源：http://jn.muxihuayi.cn

SELECT * FROM users;
来源：http://mh.chemitech.net.cn

[Q16] 查询指定列
来源：http://ri.newstarts.cn

SELECT id, name FROM users;
来源：http://ox.lnxyls.cn

[Q17] 条件查询
来源：http://mu.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cr.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://ig.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oq.muxihuayi.cn

[Q19] 范围查询
来源：http://uu.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hc.bjjhwx.cn

[Q20] IN 列表
来源：http://rf.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bj.newstarts.cn

[Q21] 空值判断
来源：http://am.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zj.szsharing.cn

[Q22] 排序
来源：http://iz.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dv.521024.cn

[Q23] 分页
来源：http://nf.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tm.bookmarksfly.cn

[Q24] 去重
来源：http://mt.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://fk.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://lc.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ej.hnjuh.cn

[Q26] 计数
来源：http://vt.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://tn.huanxung.cn

[Q27] 条件计数
来源：http://td.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fq.bookmarksfly.cn

[Q28] 求和与平均
来源：http://ke.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nu.bjjhwx.cn

[Q29] 最大最小值
来源：http://km.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cq.shxzukj.cn

[Q30] 分组统计
来源：http://gr.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wt.szxytkj.cn

[Q31] 分组后过滤
来源：http://hf.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wf.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://oc.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fb.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xv.shxzskj.cn

[Q33] 多列分组
来源：http://ae.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ov.panjiajie.cn

[Q34] 每组取第一条
来源：http://sr.shxzukj.cn

SELECT * FROM (
来源：http://ln.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vr.haigaiapp.cn

) t WHERE rn = 1;
来源：http://xc.wgjwhj.cn

[Q35] 内连接
来源：http://bd.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oh.hnjuh.cn

[Q36] 左连接
来源：http://dk.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sv.muxihuayi.cn

[Q37] 右连接
来源：http://ck.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wl.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pf.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ys.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://wr.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xt.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zd.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pl.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ge.bookmarksfly.cn

[Q41] 多表连接
来源：http://eu.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tq.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://jo.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://st.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://kk.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://yq.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yn.szxytkj.cn

[Q43] 标量子查询
来源：http://cx.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fk.huanxung.cn

[Q44] IN 子查询
来源：http://ax.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ii.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://oz.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://id.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yj.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qy.nicolike.cn

[Q47] 与平均值比较
来源：http://nf.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kj.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://gy.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://an.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://fe.521024.cn

[Q49] 更新单行
来源：http://hm.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ha.nszjky.cn

[Q50] 批量更新
来源：http://nd.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cc.szxytkj.cn

[Q51] 用子查询更新
来源：http://cm.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iu.wgjwhj.cn

[Q52] 删除指定行
来源：http://lb.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://gg.huanxung.cn

[Q53] 按条件删除
来源：http://vx.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cq.colortex.cn

[Q54] 清空表
来源：http://ie.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://th.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://mu.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sr.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://qh.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ry.newstarts.cn

[Q57] 行号
来源：http://mr.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ev.shxzukj.cn

[Q58] 累计求和
来源：http://dr.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cw.hnjuh.cn

[Q59] 分组内累计
来源：http://dc.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sf.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://id.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ml.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://df.bjjhwx.cn

[Q61] 移动平均
来源：http://ib.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nl.bookmarksfly.cn

[Q62] 分组占比
来源：http://id.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ho.muxihuayi.cn

[Q63] 开启事务
来源：http://hf.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://at.szsharing.cn

[Q64] 提交事务
来源：http://po.asd995.cn

COMMIT;
来源：http://dz.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://sp.bookmarksfly.cn

ROLLBACK;
来源：http://ce.nszjky.cn

[Q66] 行锁查询
来源：http://jh.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bc.lnxyls.cn

[Q67] 设置隔离级别
来源：http://ok.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hg.huanxung.cn

[Q68] 保存点
来源：http://eg.haigaiapp.cn

SAVEPOINT sp1;
来源：http://cx.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://pe.521024.cn

[Q69] 查看执行计划
来源：http://al.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ck.asd995.cn

[Q70] 更新统计信息
来源：http://qj.colortex.cn

ANALYZE TABLE users;
来源：http://sd.wgjwhj.cn

[Q71] 查看建表语句
来源：http://ha.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://we.szxytkj.cn

[Q72] 查看索引
来源：http://nz.panjiajie.cn


<!-- 参考信息 -->