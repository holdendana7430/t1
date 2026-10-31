代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://au.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://em.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hf.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bv.panjiajie.cn

================================================================================
来源：http://gk.shtwfgs.cn

O. 并发与异步
来源：http://oq.newstarts.cn

================================================================================
来源：http://fv.huixiangedu.cn

[O01] 启动一个线程
来源：http://xr.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oz.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xa.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hi.gzmigu.cn

TS:   // 同 JS
来源：http://gv.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://wj.szsharing.cn

Go:   go f()
来源：http://bi.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://gu.newstarts.cn

C#:   Task.Run(() => F());
来源：http://qt.yuntaijiaju.cn

[O02] 使用线程池
来源：http://qk.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://id.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kf.colortex.cn

JS:   // worker_threads 线程池
来源：http://xy.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://sx.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ns.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dv.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sz.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zn.hahajie.cn

[O03] 加锁保护共享数据
来源：http://ra.panjiajie.cn

Py:   with lock: shared += 1
来源：http://rl.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://fn.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ag.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ur.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://pu.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uo.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ih.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://du.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://xm.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://mo.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iv.asd995.cn

JS:   async function f() { await g(); }
来源：http://vm.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fn.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tz.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fv.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nj.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://wx.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://vq.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://al.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://je.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://fj.asd995.cn

TS:   await Promise.all(tasks)
来源：http://nw.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ko.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oo.9csxet.cn

Ruby: threads.map(&:join)
来源：http://db.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mt.lnxyls.cn

[O06] 使用进程池
来源：http://gu.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qz.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zo.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://dn.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://lx.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bp.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zs.hnjuh.cn

Ruby: // fork 块
来源：http://wu.huixiangedu.cn

C#:   Parallel.For
来源：http://ea.yuntaijiaju.cn

================================================================================
来源：http://xt.yuntaijiaju.cn

P. 常用工具函数
来源：http://tm.shtwfgs.cn

================================================================================
来源：http://rr.jctech888.com.cn

[P01] 生成 UUID
来源：http://yc.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://tq.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tk.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://it.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://bm.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://xw.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://yk.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ve.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://oe.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://cc.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://py.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sr.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fo.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bg.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yh.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jq.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ti.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cf.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://en.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wn.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ma.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rg.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bd.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ud.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fy.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rv.lnxyls.cn

[P04] 求长度
来源：http://dg.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fu.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cz.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zq.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vi.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://fy.nicolike.cn

Go:   len(arr);  len(m)
来源：http://pm.nicolike.cn

Ruby: x.length;  x.size
来源：http://ef.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ig.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://da.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://du.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dv.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cp.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bi.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ms.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tf.huixiangedu.cn

Ruby: a == b
来源：http://zn.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lw.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gg.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wx.asd995.cn

PHP:  if (empty($x)) {}
来源：http://em.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jf.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://lk.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zq.yuexingan06.cn

Go:   if x == nil {}
来源：http://kw.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ou.shxzskj.cn

C#:   if (x is null) {}
来源：http://xs.panjiajie.cn

[P07] 防抖与节流
来源：http://xv.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wz.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://of.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fs.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cw.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dx.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hy.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qo.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uu.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://rq.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cw.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gy.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ld.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ug.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vs.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oe.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qh.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lq.gzmigu.cn

================================================================================
来源：http://da.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ra.shxzukj.cn

================================================================================
来源：http://ql.shxzskj.cn

[Q01] 创建表
来源：http://qp.nszjky.cn

CREATE TABLE users (
来源：http://fe.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ez.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://hy.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://qq.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qh.huanxung.cn

);
来源：http://pj.huanxung.cn

[Q02] 创建带外键的表
来源：http://st.lnxyls.cn

CREATE TABLE orders (
来源：http://zp.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vi.nicolike.cn

user_id INT NOT NULL,
来源：http://yk.huanxung.cn

amount DECIMAL(10, 2),
来源：http://qg.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rq.521024.cn

);
来源：http://tc.bookmarksfly.cn

[Q03] 增加列
来源：http://kj.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ku.lnxyls.cn

[Q04] 修改列类型
来源：http://pe.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lt.newstarts.cn

[Q05] 重命名列
来源：http://ve.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://td.shxzskj.cn

[Q06] 删除列
来源：http://zy.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vz.panjiajie.cn

[Q07] 删除表
来源：http://hq.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://lf.huanxung.cn

[Q08] 创建普通索引
来源：http://qz.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vj.nszjky.cn

[Q09] 创建唯一索引
来源：http://gy.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ha.huanxung.cn

[Q10] 插入单行
来源：http://tz.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yc.szxytkj.cn

[Q11] 一次插入多行
来源：http://bv.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jc.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://wl.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jm.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vv.huanxung.cn

[Q13] 忽略重复插入
来源：http://yt.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ne.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://xq.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ws.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bm.jctech888.com.cn

[Q15] 查询全部
来源：http://xv.bookmarksfly.cn

SELECT * FROM users;
来源：http://or.9csxet.cn

[Q16] 查询指定列
来源：http://si.jctech888.com.cn

SELECT id, name FROM users;
来源：http://pu.yuntaijiaju.cn

[Q17] 条件查询
来源：http://lh.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zs.nszjky.cn

[Q18] 模糊匹配
来源：http://vx.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qv.huanxung.cn

[Q19] 范围查询
来源：http://nr.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oj.hnjuh.cn

[Q20] IN 列表
来源：http://ih.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cy.colortex.cn

[Q21] 空值判断
来源：http://vw.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kz.jianghongdianzi.cn

[Q22] 排序
来源：http://rp.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yj.shtwfgs.cn

[Q23] 分页
来源：http://kh.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mr.bjjhwx.cn

[Q24] 去重
来源：http://jd.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://cc.asd995.cn

[Q25] 只取前 N 条
来源：http://qp.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cq.bookmarksfly.cn

[Q26] 计数
来源：http://dr.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://ox.9csxet.cn

[Q27] 条件计数
来源：http://mw.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xc.szsharing.cn

[Q28] 求和与平均
来源：http://jz.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mf.lnxyls.cn

[Q29] 最大最小值
来源：http://qu.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ln.asd995.cn

[Q30] 分组统计
来源：http://ne.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ln.lnxyls.cn

[Q31] 分组后过滤
来源：http://yo.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://da.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://km.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yj.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://us.nszjky.cn

[Q33] 多列分组
来源：http://vu.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yy.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://uq.521024.cn

SELECT * FROM (
来源：http://za.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ir.muxihuayi.cn

) t WHERE rn = 1;
来源：http://fn.yuntaijiaju.cn

[Q35] 内连接
来源：http://td.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gt.bookmarksfly.cn

[Q36] 左连接
来源：http://fh.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iv.521024.cn

[Q37] 右连接
来源：http://rd.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://va.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mz.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qj.asd995.cn

[Q39] 自连接（查上下级）
来源：http://tb.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://za.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cd.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xl.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://id.colortex.cn

[Q41] 多表连接
来源：http://hy.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ig.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://up.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://gm.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://hw.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ii.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ra.nszjky.cn

[Q43] 标量子查询
来源：http://yv.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uy.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://fw.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fm.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://dg.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://np.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cq.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qm.szsharing.cn

[Q47] 与平均值比较
来源：http://gs.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cd.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://ps.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wm.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://an.gzmigu.cn

[Q49] 更新单行
来源：http://dx.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ux.hahajie.cn

[Q50] 批量更新
来源：http://sc.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ot.szsharing.cn

[Q51] 用子查询更新
来源：http://sf.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xi.hahajie.cn

[Q52] 删除指定行
来源：http://wq.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://de.521024.cn

[Q53] 按条件删除
来源：http://xk.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rh.colortex.cn

[Q54] 清空表
来源：http://tm.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://pg.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://dz.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fs.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://iu.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bm.bjjhwx.cn

[Q57] 行号
来源：http://wa.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://om.jctech888.com.cn

[Q58] 累计求和
来源：http://kj.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hl.lnxyls.cn

[Q59] 分组内累计
来源：http://vm.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sb.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://xg.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pg.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xv.colortex.cn

[Q61] 移动平均
来源：http://th.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gj.nicolike.cn

[Q62] 分组占比
来源：http://fa.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qs.colortex.cn

[Q63] 开启事务
来源：http://sx.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nb.hnjuh.cn

[Q64] 提交事务
来源：http://fp.muxihuayi.cn

COMMIT;
来源：http://fh.newstarts.cn

[Q65] 回滚事务
来源：http://td.huixiangedu.cn

ROLLBACK;
来源：http://ut.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://cb.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ya.shxzskj.cn

[Q67] 设置隔离级别
来源：http://eo.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wu.shxzskj.cn

[Q68] 保存点
来源：http://ie.wgjwhj.cn

SAVEPOINT sp1;
来源：http://mo.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://wo.nszjky.cn

[Q69] 查看执行计划
来源：http://oz.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vj.nicolike.cn

[Q70] 更新统计信息
来源：http://fg.huixinmuqiang.cn


<!-- 参考信息 -->