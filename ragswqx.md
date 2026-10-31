代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mt.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pl.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.szsharing.cn

================================================================================
来源：http://eu.521024.cn

O. 并发与异步
来源：http://ls.asd995.cn

================================================================================
来源：http://bl.bjjhwx.cn

[O01] 启动一个线程
来源：http://kc.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rx.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yj.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fn.shxzukj.cn

TS:   // 同 JS
来源：http://nz.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://wj.asd995.cn

Go:   go f()
来源：http://mx.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://vr.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://wl.haigaiapp.cn

[O02] 使用线程池
来源：http://hy.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yr.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zh.nszjky.cn

JS:   // worker_threads 线程池
来源：http://ei.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://kg.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vi.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ha.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ry.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lk.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://xu.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://xx.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://kh.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nn.newstarts.cn

TS:   // 同 JS
来源：http://ta.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://re.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gg.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yk.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://tj.szsharing.cn

[O04] 定义异步函数并等待
来源：http://be.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://tt.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gt.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://ff.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ka.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nt.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ly.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ha.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://jb.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://uy.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://vu.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mv.colortex.cn

JS:   await Promise.all(tasks)
来源：http://bc.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://sv.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mk.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://by.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://mt.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xm.shxzskj.cn

[O06] 使用进程池
来源：http://du.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qm.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mr.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://sp.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://zv.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://po.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dy.yuexingan06.cn

Ruby: // fork 块
来源：http://pj.huanxung.cn

C#:   Parallel.For
来源：http://iw.asd995.cn

================================================================================
来源：http://zo.gzmigu.cn

P. 常用工具函数
来源：http://pl.shxzskj.cn

================================================================================
来源：http://do.wgjwhj.cn

[P01] 生成 UUID
来源：http://ut.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://ci.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jv.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ua.nicolike.cn

TS:   crypto.randomUUID()
来源：http://il.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://ol.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://tg.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://fo.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://ku.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://vz.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yo.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://af.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dv.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nd.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cd.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gg.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jg.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tn.shxzskj.cn

[P03] 生成短随机字符串
来源：http://cu.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ak.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pg.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pd.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ie.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pu.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bw.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mg.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ah.jianghongdianzi.cn

[P04] 求长度
来源：http://gs.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://id.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fm.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tu.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wl.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://jy.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://sx.newstarts.cn

Ruby: x.length;  x.size
来源：http://vw.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://go.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://gb.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uw.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yi.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rw.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mj.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mr.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wn.shxzukj.cn

Ruby: a == b
来源：http://hj.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ay.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ij.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jr.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://yv.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sy.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://mo.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zr.chemitech.net.cn

Go:   if x == nil {}
来源：http://rl.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hb.shxzskj.cn

C#:   if (x is null) {}
来源：http://jn.nicolike.cn

[P07] 防抖与节流
来源：http://ey.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vl.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://ol.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hu.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gs.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vo.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://um.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://er.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eh.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://aj.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pf.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ed.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ki.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tj.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jc.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vm.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kp.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fl.shtwfgs.cn

================================================================================
来源：http://bc.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qj.huixinmuqiang.cn

================================================================================
来源：http://cq.shtwfgs.cn

[Q01] 创建表
来源：http://hv.lnxyls.cn

CREATE TABLE users (
来源：http://th.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://kx.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://ce.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wr.shxzukj.cn

);
来源：http://pi.nszjky.cn

[Q02] 创建带外键的表
来源：http://yg.hahajie.cn

CREATE TABLE orders (
来源：http://kj.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jw.colortex.cn

user_id INT NOT NULL,
来源：http://ph.hahajie.cn

amount DECIMAL(10, 2),
来源：http://jz.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tv.szsharing.cn

);
来源：http://oq.lnxyls.cn

[Q03] 增加列
来源：http://pj.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bp.gzmigu.cn

[Q04] 修改列类型
来源：http://hd.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dl.muxihuayi.cn

[Q05] 重命名列
来源：http://ng.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ar.huanxung.cn

[Q06] 删除列
来源：http://nr.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yn.bookmarksfly.cn

[Q07] 删除表
来源：http://fi.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://xa.colortex.cn

[Q08] 创建普通索引
来源：http://ol.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iq.shxzskj.cn

[Q09] 创建唯一索引
来源：http://qj.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qq.haigaiapp.cn

[Q10] 插入单行
来源：http://mp.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dc.muxihuayi.cn

[Q11] 一次插入多行
来源：http://oa.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ec.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://se.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uc.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ia.gzmigu.cn

[Q13] 忽略重复插入
来源：http://qy.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hs.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://jv.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ml.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vh.huixinmuqiang.cn

[Q15] 查询全部
来源：http://ix.gzmigu.cn

SELECT * FROM users;
来源：http://lu.huixiangedu.cn

[Q16] 查询指定列
来源：http://jz.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://py.haigaiapp.cn

[Q17] 条件查询
来源：http://jl.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gu.gzmigu.cn

[Q18] 模糊匹配
来源：http://bz.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ou.newstarts.cn

[Q19] 范围查询
来源：http://xd.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lv.hahajie.cn

[Q20] IN 列表
来源：http://qz.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ll.9csxet.cn

[Q21] 空值判断
来源：http://db.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jx.huixinmuqiang.cn

[Q22] 排序
来源：http://xg.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dl.szsharing.cn

[Q23] 分页
来源：http://ho.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gq.huixiangedu.cn

[Q24] 去重
来源：http://sb.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://rp.521024.cn

[Q25] 只取前 N 条
来源：http://gz.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dj.9csxet.cn

[Q26] 计数
来源：http://vo.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://aj.9csxet.cn

[Q27] 条件计数
来源：http://ks.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mz.haigaiapp.cn

[Q28] 求和与平均
来源：http://xb.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uz.szxytkj.cn

[Q29] 最大最小值
来源：http://ev.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gr.nszjky.cn

[Q30] 分组统计
来源：http://tb.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cx.chemitech.net.cn

[Q31] 分组后过滤
来源：http://zp.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ls.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://pf.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kt.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ky.jianghongdianzi.cn

[Q33] 多列分组
来源：http://sp.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ko.huanxung.cn

[Q34] 每组取第一条
来源：http://cd.huixiangedu.cn

SELECT * FROM (
来源：http://wv.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://am.chemitech.net.cn

) t WHERE rn = 1;
来源：http://pj.bookmarksfly.cn

[Q35] 内连接
来源：http://aq.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hh.shxzukj.cn

[Q36] 左连接
来源：http://be.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sk.yuntaijiaju.cn

[Q37] 右连接
来源：http://pq.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rx.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sq.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oi.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://wx.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nx.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kt.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dg.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bc.gzmigu.cn

[Q41] 多表连接
来源：http://ua.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bw.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://kp.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://dy.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://ry.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://rf.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zz.asd995.cn

[Q43] 标量子查询
来源：http://yp.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://on.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://wr.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yp.521024.cn

[Q45] EXISTS 判断存在
来源：http://uj.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xu.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lg.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jh.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ef.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nd.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://qf.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://em.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://os.shxzskj.cn

[Q49] 更新单行
来源：http://bj.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://np.shxzukj.cn

[Q50] 批量更新
来源：http://ju.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qm.hnjuh.cn

[Q51] 用子查询更新
来源：http://qz.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sd.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://ap.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://yx.newstarts.cn

[Q53] 按条件删除
来源：http://qu.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://an.huixiangedu.cn

[Q54] 清空表
来源：http://xf.521024.cn

TRUNCATE TABLE logs;
来源：http://oa.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://oq.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xt.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://dp.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tg.yuntaijiaju.cn

[Q57] 行号
来源：http://xf.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xz.chemitech.net.cn

[Q58] 累计求和
来源：http://vc.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jz.521024.cn

[Q59] 分组内累计
来源：http://vg.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://to.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://df.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yc.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cl.newstarts.cn

[Q61] 移动平均
来源：http://bp.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ht.bjjhwx.cn

[Q62] 分组占比
来源：http://wt.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qj.nszjky.cn

[Q63] 开启事务
来源：http://ue.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://di.gzmigu.cn

[Q64] 提交事务
来源：http://lc.muxihuayi.cn

COMMIT;
来源：http://vm.bjjhwx.cn

[Q65] 回滚事务
来源：http://md.shxzskj.cn

ROLLBACK;
来源：http://tg.521024.cn

[Q66] 行锁查询
来源：http://qu.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://se.colortex.cn

[Q67] 设置隔离级别
来源：http://tb.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qm.nszjky.cn

[Q68] 保存点
来源：http://jd.wgjwhj.cn

SAVEPOINT sp1;
来源：http://sy.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://pw.lnxyls.cn

[Q69] 查看执行计划
来源：http://zs.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xm.szsharing.cn

[Q70] 更新统计信息
来源：http://gh.jctech888.com.cn


<!-- 参考信息 -->