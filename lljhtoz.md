代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wa.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sk.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mh.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.yuexingan06.cn

================================================================================
来源：http://qc.bjjhwx.cn

O. 并发与异步
来源：http://ia.shtwfgs.cn

================================================================================
来源：http://uw.bookmarksfly.cn

[O01] 启动一个线程
来源：http://ac.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ee.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://so.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rb.huixinmuqiang.cn

TS:   // 同 JS
来源：http://dk.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://qn.colortex.cn

Go:   go f()
来源：http://du.gzmigu.cn

Ruby: Thread.new { f }
来源：http://fj.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://ju.yuexingan06.cn

[O02] 使用线程池
来源：http://db.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fn.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pw.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://tv.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://ww.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wm.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vk.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ks.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ig.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://ob.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://nq.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://ax.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ga.wgjwhj.cn

TS:   // 同 JS
来源：http://fd.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://ye.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ud.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pc.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://vj.9csxet.cn

[O04] 定义异步函数并等待
来源：http://qo.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://cd.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qd.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://dq.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wh.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ke.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xx.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://is.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://um.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://ac.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://uk.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://od.colortex.cn

JS:   await Promise.all(tasks)
来源：http://yn.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://ld.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tl.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vf.nicolike.cn

Ruby: threads.map(&:join)
来源：http://fu.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pc.521024.cn

[O06] 使用进程池
来源：http://zk.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lw.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://es.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://zp.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://dk.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://km.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pk.shxzukj.cn

Ruby: // fork 块
来源：http://la.yuexingan06.cn

C#:   Parallel.For
来源：http://vx.huixiangedu.cn

================================================================================
来源：http://fk.gzmigu.cn

P. 常用工具函数
来源：http://vo.521024.cn

================================================================================
来源：http://nr.huixiangedu.cn

[P01] 生成 UUID
来源：http://fx.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://hj.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://so.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://hn.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://jl.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://eo.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://ka.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://gr.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://yw.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://tc.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wa.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eb.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dn.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ho.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wg.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yv.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://st.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rl.colortex.cn

[P03] 生成短随机字符串
来源：http://rg.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aj.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ch.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mv.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xo.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://if.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lw.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://um.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nb.bookmarksfly.cn

[P04] 求长度
来源：http://qd.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vr.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tn.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cw.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qf.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://dp.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://gh.nicolike.cn

Ruby: x.length;  x.size
来源：http://jl.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eb.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://dl.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zn.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yq.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ct.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pc.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xa.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qg.yuntaijiaju.cn

Ruby: a == b
来源：http://ws.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ab.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wb.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rc.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://rk.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ic.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://qh.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dw.asd995.cn

Go:   if x == nil {}
来源：http://ps.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lh.nicolike.cn

C#:   if (x is null) {}
来源：http://cn.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://ef.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cw.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ln.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bb.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yl.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qi.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ry.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gi.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://to.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://vs.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oj.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://re.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yy.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zn.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ec.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bc.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://md.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sm.521024.cn

================================================================================
来源：http://xa.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xx.colortex.cn

================================================================================
来源：http://yf.colortex.cn

[Q01] 创建表
来源：http://qn.huixiangedu.cn

CREATE TABLE users (
来源：http://uv.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lx.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://ef.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://vb.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://av.szxytkj.cn

);
来源：http://ra.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://vs.lnxyls.cn

CREATE TABLE orders (
来源：http://xh.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://co.hnjuh.cn

user_id INT NOT NULL,
来源：http://tu.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://zo.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hb.yuntaijiaju.cn

);
来源：http://kl.521024.cn

[Q03] 增加列
来源：http://zo.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://le.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://lw.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qh.nicolike.cn

[Q05] 重命名列
来源：http://ew.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sn.nicolike.cn

[Q06] 删除列
来源：http://yr.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ur.bookmarksfly.cn

[Q07] 删除表
来源：http://vn.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://fy.huanxung.cn

[Q08] 创建普通索引
来源：http://jv.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ta.gzmigu.cn

[Q09] 创建唯一索引
来源：http://am.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fm.asd995.cn

[Q10] 插入单行
来源：http://vf.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ic.haigaiapp.cn

[Q11] 一次插入多行
来源：http://wo.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zu.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://kh.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://im.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oh.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://mj.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://da.521024.cn

[Q14] 存在则更新（upsert）
来源：http://jd.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ux.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fj.bjjhwx.cn

[Q15] 查询全部
来源：http://wh.bookmarksfly.cn

SELECT * FROM users;
来源：http://zv.gzmigu.cn

[Q16] 查询指定列
来源：http://lq.hahajie.cn

SELECT id, name FROM users;
来源：http://ce.shxzukj.cn

[Q17] 条件查询
来源：http://eu.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cm.chemitech.net.cn

[Q18] 模糊匹配
来源：http://yb.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://us.shxzskj.cn

[Q19] 范围查询
来源：http://lp.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qk.yuexingan06.cn

[Q20] IN 列表
来源：http://gx.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ig.szxytkj.cn

[Q21] 空值判断
来源：http://tj.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ym.hnjuh.cn

[Q22] 排序
来源：http://ts.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zb.nszjky.cn

[Q23] 分页
来源：http://sa.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vz.lnxyls.cn

[Q24] 去重
来源：http://gg.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://ka.huanxung.cn

[Q25] 只取前 N 条
来源：http://fq.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ev.9csxet.cn

[Q26] 计数
来源：http://dj.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://us.haigaiapp.cn

[Q27] 条件计数
来源：http://mc.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ww.szxytkj.cn

[Q28] 求和与平均
来源：http://mt.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jj.lnxyls.cn

[Q29] 最大最小值
来源：http://vo.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wb.nicolike.cn

[Q30] 分组统计
来源：http://ak.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dj.9csxet.cn

[Q31] 分组后过滤
来源：http://sl.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yn.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://hv.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ie.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://np.muxihuayi.cn

[Q33] 多列分组
来源：http://ny.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ba.jctech888.com.cn

[Q34] 每组取第一条
来源：http://ec.colortex.cn

SELECT * FROM (
来源：http://lh.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mo.shxzskj.cn

) t WHERE rn = 1;
来源：http://al.wgjwhj.cn

[Q35] 内连接
来源：http://iy.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ch.shxzukj.cn

[Q36] 左连接
来源：http://px.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yv.bookmarksfly.cn

[Q37] 右连接
来源：http://ty.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ri.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pd.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vl.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://hb.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ln.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rt.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://td.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ef.colortex.cn

[Q41] 多表连接
来源：http://wv.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sp.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://zw.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://sv.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://te.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://gs.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ke.muxihuayi.cn

[Q43] 标量子查询
来源：http://fm.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ne.szsharing.cn

[Q44] IN 子查询
来源：http://dl.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jp.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://si.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fm.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yy.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://me.bjjhwx.cn

[Q47] 与平均值比较
来源：http://eb.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mb.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://bh.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wd.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://kd.nszjky.cn

[Q49] 更新单行
来源：http://jx.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zd.nszjky.cn

[Q50] 批量更新
来源：http://ur.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wm.chemitech.net.cn

[Q51] 用子查询更新
来源：http://ms.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jp.bjjhwx.cn

[Q52] 删除指定行
来源：http://mu.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://ss.lnxyls.cn

[Q53] 按条件删除
来源：http://ce.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ax.newstarts.cn

[Q54] 清空表
来源：http://wv.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://sh.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://av.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ol.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://xb.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sk.newstarts.cn

[Q57] 行号
来源：http://bi.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qh.colortex.cn

[Q58] 累计求和
来源：http://uf.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://en.jctech888.com.cn

[Q59] 分组内累计
来源：http://hh.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wt.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://iw.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://os.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ah.jianghongdianzi.cn

[Q61] 移动平均
来源：http://wz.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rk.panjiajie.cn

[Q62] 分组占比
来源：http://zn.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uv.shxzukj.cn

[Q63] 开启事务
来源：http://rs.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://db.huixinmuqiang.cn

[Q64] 提交事务
来源：http://qj.huixiangedu.cn

COMMIT;
来源：http://zy.jctech888.com.cn

[Q65] 回滚事务
来源：http://kh.huanxung.cn

ROLLBACK;
来源：http://rn.shtwfgs.cn

[Q66] 行锁查询
来源：http://hi.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zy.asd995.cn

[Q67] 设置隔离级别
来源：http://fs.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pa.yuntaijiaju.cn

[Q68] 保存点
来源：http://aw.shxzskj.cn

SAVEPOINT sp1;
来源：http://wt.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://cl.haigaiapp.cn

[Q69] 查看执行计划
来源：http://oi.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hw.muxihuayi.cn

[Q70] 更新统计信息
来源：http://eu.szsharing.cn


<!-- 参考信息 -->