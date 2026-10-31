代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zo.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ik.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lu.colortex.cn

TS:   // 同 JS
来源：http://cg.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://tr.asd995.cn

Go:   go f()
来源：http://hd.colortex.cn

Ruby: Thread.new { f }
来源：http://nq.newstarts.cn

C#:   Task.Run(() => F());
来源：http://qq.szxytkj.cn

[O02] 使用线程池
来源：http://yg.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mp.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vw.colortex.cn

JS:   // worker_threads 线程池
来源：http://ai.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://ti.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lw.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lk.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://er.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://td.asd995.cn

[O03] 加锁保护共享数据
来源：http://cu.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://ks.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://ds.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dc.yuntaijiaju.cn

TS:   // 同 JS
来源：http://eg.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://pv.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qz.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cp.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://an.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://yc.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://lt.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ea.colortex.cn

JS:   async function f() { await g(); }
来源：http://wu.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uj.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mk.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rf.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cn.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://uq.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://ty.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://mh.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uq.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://od.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://hx.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vs.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qd.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ch.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hv.muxihuayi.cn

[O06] 使用进程池
来源：http://cs.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://op.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://da.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://cy.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://yf.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lt.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wz.jianghongdianzi.cn

Ruby: // fork 块
来源：http://eo.521024.cn

C#:   Parallel.For
来源：http://mq.asd995.cn

================================================================================
来源：http://wh.9csxet.cn

P. 常用工具函数
来源：http://yb.asd995.cn

================================================================================
来源：http://tu.yuexingan06.cn

[P01] 生成 UUID
来源：http://ke.asd995.cn

Py:   str(uuid.uuid4())
来源：http://fr.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://io.9csxet.cn

JS:   crypto.randomUUID()
来源：http://pu.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://sw.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://et.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://eh.colortex.cn

Ruby: SecureRandom.uuid
来源：http://gs.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://jp.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://av.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uo.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ur.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ss.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pd.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vb.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xu.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ph.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cv.521024.cn

[P03] 生成短随机字符串
来源：http://vn.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://br.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gp.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ai.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mr.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wj.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ls.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rj.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kc.hahajie.cn

[P04] 求长度
来源：http://yj.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nv.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uq.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cn.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://bv.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://bz.panjiajie.cn

Ruby: x.length;  x.size
来源：http://ad.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mk.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://za.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yz.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nw.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jn.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ko.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cz.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://en.gzmigu.cn

Ruby: a == b
来源：http://kp.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cc.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xm.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sz.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://ie.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ht.shxzukj.cn

TS:   if (x == null) {}
来源：http://mp.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pq.yuexingan06.cn

Go:   if x == nil {}
来源：http://ow.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lg.wgjwhj.cn

C#:   if (x is null) {}
来源：http://lz.wgjwhj.cn

[P07] 防抖与节流
来源：http://ie.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ej.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://gj.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kh.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://by.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fx.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pc.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gs.huanxung.cn

[P08] 处理浮点精度问题
来源：http://sj.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ua.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mh.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qq.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nl.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mk.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fm.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pl.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nr.muxihuayi.cn

================================================================================
来源：http://tg.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mx.521024.cn

================================================================================
来源：http://wa.newstarts.cn

[Q01] 创建表
来源：http://oy.huixinmuqiang.cn

CREATE TABLE users (
来源：http://cb.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bm.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://nw.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://xo.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zr.huixiangedu.cn

);
来源：http://oh.colortex.cn

[Q02] 创建带外键的表
来源：http://px.szsharing.cn

CREATE TABLE orders (
来源：http://zi.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uj.bjjhwx.cn

user_id INT NOT NULL,
来源：http://vi.szsharing.cn

amount DECIMAL(10, 2),
来源：http://dm.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://il.hahajie.cn

);
来源：http://gr.huixinmuqiang.cn

[Q03] 增加列
来源：http://qc.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nq.jctech888.com.cn

[Q04] 修改列类型
来源：http://wg.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qn.shxzskj.cn

[Q05] 重命名列
来源：http://gs.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dn.jianghongdianzi.cn

[Q06] 删除列
来源：http://uz.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wg.szxytkj.cn

[Q07] 删除表
来源：http://vo.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://wl.szsharing.cn

[Q08] 创建普通索引
来源：http://xn.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pz.colortex.cn

[Q09] 创建唯一索引
来源：http://fu.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uj.shxzskj.cn

[Q10] 插入单行
来源：http://ll.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jb.shxzskj.cn

[Q11] 一次插入多行
来源：http://dy.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tp.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://th.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://li.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dq.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://wo.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cq.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://by.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rc.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bj.haigaiapp.cn

[Q15] 查询全部
来源：http://ak.lnxyls.cn

SELECT * FROM users;
来源：http://mn.panjiajie.cn

[Q16] 查询指定列
来源：http://xh.haigaiapp.cn

SELECT id, name FROM users;
来源：http://ev.bookmarksfly.cn

[Q17] 条件查询
来源：http://zt.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bn.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://jr.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ga.chemitech.net.cn

[Q19] 范围查询
来源：http://ym.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bz.huixinmuqiang.cn

[Q20] IN 列表
来源：http://jh.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rx.yuexingan06.cn

[Q21] 空值判断
来源：http://ni.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mr.bookmarksfly.cn

[Q22] 排序
来源：http://nu.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bv.hnjuh.cn

[Q23] 分页
来源：http://jv.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dc.bjjhwx.cn

[Q24] 去重
来源：http://fa.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://an.hnjuh.cn

[Q25] 只取前 N 条
来源：http://af.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hv.hahajie.cn

[Q26] 计数
来源：http://gu.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://cm.bookmarksfly.cn

[Q27] 条件计数
来源：http://oj.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ns.huixiangedu.cn

[Q28] 求和与平均
来源：http://qa.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://we.hahajie.cn

[Q29] 最大最小值
来源：http://pj.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://to.hahajie.cn

[Q30] 分组统计
来源：http://mq.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fs.shtwfgs.cn

[Q31] 分组后过滤
来源：http://dm.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ug.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://gd.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dg.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pc.panjiajie.cn

[Q33] 多列分组
来源：http://gj.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lt.9csxet.cn

[Q34] 每组取第一条
来源：http://ft.szsharing.cn

SELECT * FROM (
来源：http://mo.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rw.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://av.shtwfgs.cn

[Q35] 内连接
来源：http://qj.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://io.huixinmuqiang.cn

[Q36] 左连接
来源：http://hy.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bi.gzmigu.cn

[Q37] 右连接
来源：http://dx.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hi.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tv.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tv.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://zz.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vg.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eq.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nc.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jw.bookmarksfly.cn

[Q41] 多表连接
来源：http://ol.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lf.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://lm.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://yy.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://nz.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://vj.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ab.jctech888.com.cn

[Q43] 标量子查询
来源：http://ez.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tg.9csxet.cn

[Q44] IN 子查询
来源：http://gx.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uq.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://rk.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wj.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dc.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tt.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://fy.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ni.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://aw.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rq.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://zu.jctech888.com.cn

[Q49] 更新单行
来源：http://bk.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nn.bjjhwx.cn

[Q50] 批量更新
来源：http://pm.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uc.yuexingan06.cn

[Q51] 用子查询更新
来源：http://fl.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vr.lnxyls.cn

[Q52] 删除指定行
来源：http://ms.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://nw.asd995.cn

[Q53] 按条件删除
来源：http://ep.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ou.huixinmuqiang.cn

[Q54] 清空表
来源：http://df.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ps.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://yw.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ha.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://ri.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ln.shxzskj.cn

[Q57] 行号
来源：http://dk.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dr.jctech888.com.cn

[Q58] 累计求和
来源：http://js.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dn.shtwfgs.cn

[Q59] 分组内累计
来源：http://qv.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ts.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://ul.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ld.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tz.colortex.cn

[Q61] 移动平均
来源：http://sr.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qj.521024.cn

[Q62] 分组占比
来源：http://or.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mu.newstarts.cn

[Q63] 开启事务
来源：http://ho.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zc.nszjky.cn

[Q64] 提交事务
来源：http://ma.9csxet.cn

COMMIT;
来源：http://za.wgjwhj.cn

[Q65] 回滚事务
来源：http://oo.bookmarksfly.cn

ROLLBACK;
来源：http://ys.panjiajie.cn

[Q66] 行锁查询
来源：http://ni.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kg.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://mx.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://he.shxzskj.cn

[Q68] 保存点
来源：http://ec.muxihuayi.cn

SAVEPOINT sp1;
来源：http://nl.hnjuh.cn

ROLLBACK TO sp1;
来源：http://ds.shxzskj.cn

[Q69] 查看执行计划
来源：http://fz.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yv.szxytkj.cn

[Q70] 更新统计信息
来源：http://ox.bjjhwx.cn

ANALYZE TABLE users;
来源：http://br.huixiangedu.cn

[Q71] 查看建表语句
来源：http://ev.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hc.lnxyls.cn

[Q72] 查看索引
来源：http://hd.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://pz.chemitech.net.cn

[Q73] 查看表状态
来源：http://jh.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uv.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ql.asd995.cn


<!-- 参考信息 -->