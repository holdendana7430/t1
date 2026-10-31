代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nt.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://am.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mk.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.szxytkj.cn

================================================================================
来源：http://ou.shxzskj.cn

O. 并发与异步
来源：http://ba.asd995.cn

================================================================================
来源：http://fd.shxzukj.cn

[O01] 启动一个线程
来源：http://bg.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xe.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yr.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gv.szxytkj.cn

TS:   // 同 JS
来源：http://uz.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://yb.szxytkj.cn

Go:   go f()
来源：http://xw.panjiajie.cn

Ruby: Thread.new { f }
来源：http://ww.nszjky.cn

C#:   Task.Run(() => F());
来源：http://rd.shxzukj.cn

[O02] 使用线程池
来源：http://nj.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zr.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://um.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://eq.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://ii.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vy.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zf.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yf.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wh.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://im.shxzskj.cn

Py:   with lock: shared += 1
来源：http://mp.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://qu.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tu.yuntaijiaju.cn

TS:   // 同 JS
来源：http://br.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://pq.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://up.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jg.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://xx.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://dh.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://qx.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://az.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://xc.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jx.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ft.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xs.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vl.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://dw.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://hk.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://td.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ao.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://qy.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://eb.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fj.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bm.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ig.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qi.shtwfgs.cn

[O06] 使用进程池
来源：http://yt.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pm.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://im.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://sy.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://xs.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xs.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qr.bjjhwx.cn

Ruby: // fork 块
来源：http://lc.huanxung.cn

C#:   Parallel.For
来源：http://uh.9csxet.cn

================================================================================
来源：http://ru.newstarts.cn

P. 常用工具函数
来源：http://mo.lnxyls.cn

================================================================================
来源：http://le.nicolike.cn

[P01] 生成 UUID
来源：http://ha.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://fy.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mm.hahajie.cn

JS:   crypto.randomUUID()
来源：http://zo.hahajie.cn

TS:   crypto.randomUUID()
来源：http://zy.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://ir.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://il.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://sx.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://mn.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://em.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://by.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ta.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sm.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nm.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nf.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zf.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ks.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lq.newstarts.cn

[P03] 生成短随机字符串
来源：http://tj.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ah.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tt.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gs.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gl.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://le.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uk.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wt.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vf.bookmarksfly.cn

[P04] 求长度
来源：http://fx.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ct.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://td.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hp.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gb.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://yn.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://ki.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://oe.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sj.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://kl.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xn.hahajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://el.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://np.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rx.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ws.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dv.gzmigu.cn

Ruby: a == b
来源：http://jw.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://re.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ou.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pz.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://kg.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kv.wgjwhj.cn

TS:   if (x == null) {}
来源：http://ch.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pf.shxzskj.cn

Go:   if x == nil {}
来源：http://up.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ax.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://lb.jctech888.com.cn

[P07] 防抖与节流
来源：http://ik.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hl.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://dr.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pg.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ai.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ll.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ex.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qm.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ma.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://kp.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wx.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cr.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nh.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yy.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nm.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xh.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zx.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bw.lnxyls.cn

================================================================================
来源：http://db.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vw.asd995.cn

================================================================================
来源：http://ky.huixiangedu.cn

[Q01] 创建表
来源：http://qe.huixinmuqiang.cn

CREATE TABLE users (
来源：http://jp.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yc.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://vi.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://eg.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zx.nicolike.cn

);
来源：http://el.gzmigu.cn

[Q02] 创建带外键的表
来源：http://uj.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ri.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iv.muxihuayi.cn

user_id INT NOT NULL,
来源：http://ui.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://fx.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yq.szxytkj.cn

);
来源：http://ow.muxihuayi.cn

[Q03] 增加列
来源：http://fn.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ew.yuexingan06.cn

[Q04] 修改列类型
来源：http://xy.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wx.wgjwhj.cn

[Q05] 重命名列
来源：http://fq.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://om.szxytkj.cn

[Q06] 删除列
来源：http://nn.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ln.shxzukj.cn

[Q07] 删除表
来源：http://wf.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://mp.haigaiapp.cn

[Q08] 创建普通索引
来源：http://cx.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xp.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://sb.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://um.gzmigu.cn

[Q10] 插入单行
来源：http://kn.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://li.shxzskj.cn

[Q11] 一次插入多行
来源：http://wh.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xy.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://ag.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xx.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://th.521024.cn

[Q13] 忽略重复插入
来源：http://so.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hp.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://tu.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wk.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ij.nicolike.cn

[Q15] 查询全部
来源：http://ss.nicolike.cn

SELECT * FROM users;
来源：http://wn.bookmarksfly.cn

[Q16] 查询指定列
来源：http://xx.gzmigu.cn

SELECT id, name FROM users;
来源：http://yt.huixiangedu.cn

[Q17] 条件查询
来源：http://pd.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tl.colortex.cn

[Q18] 模糊匹配
来源：http://qs.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cp.521024.cn

[Q19] 范围查询
来源：http://qw.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lx.asd995.cn

[Q20] IN 列表
来源：http://dt.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zd.chemitech.net.cn

[Q21] 空值判断
来源：http://eb.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mj.gzmigu.cn

[Q22] 排序
来源：http://bi.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://py.nszjky.cn

[Q23] 分页
来源：http://ma.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bc.szsharing.cn

[Q24] 去重
来源：http://ka.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://hr.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://wu.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://le.szsharing.cn

[Q26] 计数
来源：http://xs.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://qa.yuexingan06.cn

[Q27] 条件计数
来源：http://cd.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xq.szsharing.cn

[Q28] 求和与平均
来源：http://wo.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xf.szsharing.cn

[Q29] 最大最小值
来源：http://mn.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pt.wgjwhj.cn

[Q30] 分组统计
来源：http://xr.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ln.haigaiapp.cn

[Q31] 分组后过滤
来源：http://fy.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uh.huanxung.cn

[Q32] 分组拼接字符串
来源：http://zg.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fy.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://va.521024.cn

[Q33] 多列分组
来源：http://xr.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dc.nszjky.cn

[Q34] 每组取第一条
来源：http://ta.hnjuh.cn

SELECT * FROM (
来源：http://sx.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hj.haigaiapp.cn

) t WHERE rn = 1;
来源：http://be.newstarts.cn

[Q35] 内连接
来源：http://vc.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fh.gzmigu.cn

[Q36] 左连接
来源：http://jn.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yi.shxzskj.cn

[Q37] 右连接
来源：http://dy.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ec.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://az.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ql.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://es.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jz.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kn.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://id.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ol.huixinmuqiang.cn

[Q41] 多表连接
来源：http://db.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://is.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://sl.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://rn.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://qs.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://bt.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://os.nicolike.cn

[Q43] 标量子查询
来源：http://aj.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kt.hnjuh.cn

[Q44] IN 子查询
来源：http://zn.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gy.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://wk.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ny.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xd.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wf.shxzskj.cn

[Q47] 与平均值比较
来源：http://qb.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vl.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://en.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yp.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://te.gzmigu.cn

[Q49] 更新单行
来源：http://ry.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yc.hnjuh.cn

[Q50] 批量更新
来源：http://tq.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://az.lnxyls.cn

[Q51] 用子查询更新
来源：http://hg.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oc.9csxet.cn

[Q52] 删除指定行
来源：http://sx.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://pf.haigaiapp.cn

[Q53] 按条件删除
来源：http://yc.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rn.nicolike.cn

[Q54] 清空表
来源：http://uv.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://in.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://tq.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yd.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://cw.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ph.gzmigu.cn

[Q57] 行号
来源：http://lg.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yp.haigaiapp.cn

[Q58] 累计求和
来源：http://yw.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fu.jctech888.com.cn

[Q59] 分组内累计
来源：http://td.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ze.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://rf.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://th.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qz.chemitech.net.cn

[Q61] 移动平均
来源：http://yq.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zf.shxzskj.cn

[Q62] 分组占比
来源：http://na.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eg.521024.cn

[Q63] 开启事务
来源：http://ro.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://om.szxytkj.cn

[Q64] 提交事务
来源：http://fe.chemitech.net.cn

COMMIT;
来源：http://dw.wgjwhj.cn

[Q65] 回滚事务
来源：http://jd.panjiajie.cn

ROLLBACK;
来源：http://pv.jctech888.com.cn

[Q66] 行锁查询
来源：http://at.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ik.panjiajie.cn

[Q67] 设置隔离级别
来源：http://vy.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uw.szxytkj.cn

[Q68] 保存点
来源：http://dp.szsharing.cn

SAVEPOINT sp1;
来源：http://ee.hahajie.cn

ROLLBACK TO sp1;
来源：http://la.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://ij.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rs.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://fs.gzmigu.cn


<!-- 参考信息 -->