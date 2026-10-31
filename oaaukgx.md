代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ce.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sf.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cd.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xm.szsharing.cn

================================================================================
来源：http://as.szxytkj.cn

O. 并发与异步
来源：http://ts.wgjwhj.cn

================================================================================
来源：http://th.bookmarksfly.cn

[O01] 启动一个线程
来源：http://nt.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jr.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jf.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ot.9csxet.cn

TS:   // 同 JS
来源：http://cy.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://la.colortex.cn

Go:   go f()
来源：http://lz.szsharing.cn

Ruby: Thread.new { f }
来源：http://le.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://rv.nszjky.cn

[O02] 使用线程池
来源：http://fp.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zj.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cs.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://bk.szsharing.cn

TS:   // worker_threads 线程池
来源：http://du.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dz.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lx.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wi.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dg.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://ts.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://dr.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://uw.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ma.muxihuayi.cn

TS:   // 同 JS
来源：http://fr.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://rs.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yc.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mc.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://wa.nszjky.cn

[O04] 定义异步函数并等待
来源：http://wd.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://ob.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oz.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://qv.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wt.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yr.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ly.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jr.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://ih.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://zc.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://jw.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://il.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://zh.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ov.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sc.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sy.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ri.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vr.haigaiapp.cn

[O06] 使用进程池
来源：http://yz.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ju.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mk.521024.cn

JS:   // child_process / cluster 模块
来源：http://ku.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://gp.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cw.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://st.szxytkj.cn

Ruby: // fork 块
来源：http://rx.wgjwhj.cn

C#:   Parallel.For
来源：http://kj.521024.cn

================================================================================
来源：http://gv.huanxung.cn

P. 常用工具函数
来源：http://jm.huixiangedu.cn

================================================================================
来源：http://cp.shxzukj.cn

[P01] 生成 UUID
来源：http://uc.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://up.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kj.asd995.cn

JS:   crypto.randomUUID()
来源：http://ub.521024.cn

TS:   crypto.randomUUID()
来源：http://hg.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://tw.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://wg.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://uv.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://yd.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://dp.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bl.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gx.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://go.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wk.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tp.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qi.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://co.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gi.asd995.cn

[P03] 生成短随机字符串
来源：http://dn.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ly.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xt.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bp.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hg.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hq.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cf.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ba.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ra.szxytkj.cn

[P04] 求长度
来源：http://qk.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nx.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://za.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mg.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xt.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://sa.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://ld.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://fh.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://om.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://wq.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ip.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iz.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lm.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fc.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://il.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pb.muxihuayi.cn

Ruby: a == b
来源：http://jb.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vm.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vi.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gx.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://jp.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qz.hnjuh.cn

TS:   if (x == null) {}
来源：http://fp.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mu.chemitech.net.cn

Go:   if x == nil {}
来源：http://tc.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://on.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://hu.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://bv.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fm.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://sd.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hj.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cz.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://js.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://su.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qn.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jr.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://cw.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fk.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nd.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ru.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://go.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kf.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iv.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eg.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xe.jianghongdianzi.cn

================================================================================
来源：http://xn.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lk.shtwfgs.cn

================================================================================
来源：http://wf.szsharing.cn

[Q01] 创建表
来源：http://aw.szsharing.cn

CREATE TABLE users (
来源：http://xe.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dp.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ti.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://we.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ax.muxihuayi.cn

);
来源：http://fd.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://se.nszjky.cn

CREATE TABLE orders (
来源：http://yh.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://co.newstarts.cn

user_id INT NOT NULL,
来源：http://dn.asd995.cn

amount DECIMAL(10, 2),
来源：http://kv.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xi.jctech888.com.cn

);
来源：http://is.521024.cn

[Q03] 增加列
来源：http://dk.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ls.asd995.cn

[Q04] 修改列类型
来源：http://wl.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xw.shtwfgs.cn

[Q05] 重命名列
来源：http://rq.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sb.521024.cn

[Q06] 删除列
来源：http://ke.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eu.hahajie.cn

[Q07] 删除表
来源：http://dg.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://vs.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://qg.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rm.9csxet.cn

[Q09] 创建唯一索引
来源：http://rt.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yh.huixinmuqiang.cn

[Q10] 插入单行
来源：http://cw.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lp.huixiangedu.cn

[Q11] 一次插入多行
来源：http://hw.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gm.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://dl.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xo.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yp.shxzukj.cn

[Q13] 忽略重复插入
来源：http://rz.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ec.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://ny.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://em.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uh.szsharing.cn

[Q15] 查询全部
来源：http://ec.hahajie.cn

SELECT * FROM users;
来源：http://ap.jctech888.com.cn

[Q16] 查询指定列
来源：http://jy.shtwfgs.cn

SELECT id, name FROM users;
来源：http://on.hahajie.cn

[Q17] 条件查询
来源：http://px.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ej.shxzukj.cn

[Q18] 模糊匹配
来源：http://zm.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kp.yuntaijiaju.cn

[Q19] 范围查询
来源：http://zx.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tc.jianghongdianzi.cn

[Q20] IN 列表
来源：http://eq.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vu.yuexingan06.cn

[Q21] 空值判断
来源：http://ct.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lt.9csxet.cn

[Q22] 排序
来源：http://ps.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xo.wgjwhj.cn

[Q23] 分页
来源：http://ef.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://da.colortex.cn

[Q24] 去重
来源：http://zi.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://hp.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://tu.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zg.szsharing.cn

[Q26] 计数
来源：http://hz.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://au.haigaiapp.cn

[Q27] 条件计数
来源：http://us.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nq.yuexingan06.cn

[Q28] 求和与平均
来源：http://ba.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tq.huixiangedu.cn

[Q29] 最大最小值
来源：http://gh.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oc.yuntaijiaju.cn

[Q30] 分组统计
来源：http://sh.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cj.nicolike.cn

[Q31] 分组后过滤
来源：http://de.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hq.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://ls.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://us.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sc.huixinmuqiang.cn

[Q33] 多列分组
来源：http://po.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zw.jctech888.com.cn

[Q34] 每组取第一条
来源：http://is.asd995.cn

SELECT * FROM (
来源：http://sn.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yx.huanxung.cn

) t WHERE rn = 1;
来源：http://jn.jianghongdianzi.cn

[Q35] 内连接
来源：http://kk.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://df.9csxet.cn

[Q36] 左连接
来源：http://di.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jy.nicolike.cn

[Q37] 右连接
来源：http://og.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ob.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uo.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gc.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://xy.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ko.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yv.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gf.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pt.newstarts.cn

[Q41] 多表连接
来源：http://cn.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gz.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://dv.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://bc.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://mq.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://nv.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mb.colortex.cn

[Q43] 标量子查询
来源：http://ow.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cg.szsharing.cn

[Q44] IN 子查询
来源：http://rv.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cd.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://kb.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nc.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ic.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ck.chemitech.net.cn

[Q47] 与平均值比较
来源：http://ie.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bz.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ev.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nt.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ih.yuexingan06.cn

[Q49] 更新单行
来源：http://lk.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zv.shxzukj.cn

[Q50] 批量更新
来源：http://vq.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xl.nicolike.cn

[Q51] 用子查询更新
来源：http://ec.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gg.521024.cn

[Q52] 删除指定行
来源：http://wi.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://ue.nszjky.cn

[Q53] 按条件删除
来源：http://ry.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sd.bjjhwx.cn

[Q54] 清空表
来源：http://vn.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://lj.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://vk.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nq.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://fy.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uu.nszjky.cn

[Q57] 行号
来源：http://oe.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vf.newstarts.cn

[Q58] 累计求和
来源：http://bh.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vi.colortex.cn

[Q59] 分组内累计
来源：http://ht.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bz.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://ps.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fc.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://in.bjjhwx.cn

[Q61] 移动平均
来源：http://nz.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jk.panjiajie.cn

[Q62] 分组占比
来源：http://hh.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xk.hahajie.cn

[Q63] 开启事务
来源：http://jf.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ch.shxzukj.cn

[Q64] 提交事务
来源：http://ig.521024.cn

COMMIT;
来源：http://jf.hahajie.cn

[Q65] 回滚事务
来源：http://jz.chemitech.net.cn

ROLLBACK;
来源：http://vl.nicolike.cn

[Q66] 行锁查询
来源：http://cf.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nn.nszjky.cn

[Q67] 设置隔离级别
来源：http://uj.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ik.9csxet.cn

[Q68] 保存点
来源：http://sk.szsharing.cn

SAVEPOINT sp1;
来源：http://xy.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://do.hahajie.cn

[Q69] 查看执行计划
来源：http://yt.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://up.chemitech.net.cn

[Q70] 更新统计信息
来源：http://eb.szsharing.cn


<!-- 参考信息 -->