代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://vb.muxihuayi.cn

Go:   go f()
来源：http://mj.nicolike.cn

Ruby: Thread.new { f }
来源：http://sc.9csxet.cn

C#:   Task.Run(() => F());
来源：http://tj.colortex.cn

[O02] 使用线程池
来源：http://ra.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lx.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bw.szsharing.cn

JS:   // worker_threads 线程池
来源：http://pm.newstarts.cn

TS:   // worker_threads 线程池
来源：http://ci.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ju.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sy.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hp.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cu.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://wn.shxzukj.cn

Py:   with lock: shared += 1
来源：http://dc.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://jf.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.bjjhwx.cn

TS:   // 同 JS
来源：http://to.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://pn.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bz.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bl.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://tv.newstarts.cn

[O04] 定义异步函数并等待
来源：http://bg.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://gs.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rf.nicolike.cn

JS:   async function f() { await g(); }
来源：http://fs.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hp.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://te.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tj.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xr.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://nu.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://om.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://aw.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ar.asd995.cn

JS:   await Promise.all(tasks)
来源：http://ts.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://kk.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vk.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wg.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://my.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aj.yuexingan06.cn

[O06] 使用进程池
来源：http://gy.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xq.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sj.asd995.cn

JS:   // child_process / cluster 模块
来源：http://tl.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://uk.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gx.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tk.huixiangedu.cn

Ruby: // fork 块
来源：http://ac.hahajie.cn

C#:   Parallel.For
来源：http://ae.bookmarksfly.cn

================================================================================
来源：http://pu.9csxet.cn

P. 常用工具函数
来源：http://gw.shtwfgs.cn

================================================================================
来源：http://po.nicolike.cn

[P01] 生成 UUID
来源：http://xh.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://jj.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pm.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://cq.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://pa.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://kn.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://aw.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://to.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ei.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://su.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hj.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ri.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wt.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://th.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ao.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dq.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ju.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pj.gzmigu.cn

[P03] 生成短随机字符串
来源：http://qb.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tp.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rx.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mp.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jb.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ml.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bv.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gh.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://if.9csxet.cn

[P04] 求长度
来源：http://lu.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xt.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jq.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zq.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ib.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://qd.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://zx.hahajie.cn

Ruby: x.length;  x.size
来源：http://bt.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ip.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://by.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ui.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nn.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mf.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sq.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nl.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xj.nszjky.cn

Ruby: a == b
来源：http://ef.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ay.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fm.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fk.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://ms.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fl.521024.cn

TS:   if (x == null) {}
来源：http://bk.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jx.shxzskj.cn

Go:   if x == nil {}
来源：http://na.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hi.yuexingan06.cn

C#:   if (x is null) {}
来源：http://uv.wgjwhj.cn

[P07] 防抖与节流
来源：http://iq.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qj.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://jn.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dr.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pd.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tf.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ox.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yw.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gz.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://ly.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tn.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gf.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bm.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gk.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ed.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ly.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dk.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ag.gzmigu.cn

================================================================================
来源：http://lb.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kw.panjiajie.cn

================================================================================
来源：http://iy.szsharing.cn

[Q01] 创建表
来源：http://yu.shxzukj.cn

CREATE TABLE users (
来源：http://mm.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ac.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://yg.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://gd.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sz.szsharing.cn

);
来源：http://ib.huanxung.cn

[Q02] 创建带外键的表
来源：http://oq.bookmarksfly.cn

CREATE TABLE orders (
来源：http://fs.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lm.wgjwhj.cn

user_id INT NOT NULL,
来源：http://wq.nicolike.cn

amount DECIMAL(10, 2),
来源：http://ux.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yu.panjiajie.cn

);
来源：http://pk.nszjky.cn

[Q03] 增加列
来源：http://eh.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qf.nszjky.cn

[Q04] 修改列类型
来源：http://yw.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://so.9csxet.cn

[Q05] 重命名列
来源：http://us.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://my.chemitech.net.cn

[Q06] 删除列
来源：http://dy.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pq.szxytkj.cn

[Q07] 删除表
来源：http://jp.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://dc.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://dn.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://co.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://pk.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fm.bjjhwx.cn

[Q10] 插入单行
来源：http://pa.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xf.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://vz.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ha.colortex.cn

[Q12] 插入后取自增 ID
来源：http://ju.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ov.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mn.huanxung.cn

[Q13] 忽略重复插入
来源：http://um.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pb.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://di.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pl.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ue.huixiangedu.cn

[Q15] 查询全部
来源：http://im.huixinmuqiang.cn

SELECT * FROM users;
来源：http://nu.huixiangedu.cn

[Q16] 查询指定列
来源：http://re.shtwfgs.cn

SELECT id, name FROM users;
来源：http://eq.shtwfgs.cn

[Q17] 条件查询
来源：http://zq.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fg.wgjwhj.cn

[Q18] 模糊匹配
来源：http://nd.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cx.yuntaijiaju.cn

[Q19] 范围查询
来源：http://hb.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mw.colortex.cn

[Q20] IN 列表
来源：http://xq.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ds.huixinmuqiang.cn

[Q21] 空值判断
来源：http://au.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jg.9csxet.cn

[Q22] 排序
来源：http://ro.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xa.huixiangedu.cn

[Q23] 分页
来源：http://er.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hf.yuexingan06.cn

[Q24] 去重
来源：http://gv.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ol.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://qd.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xd.muxihuayi.cn

[Q26] 计数
来源：http://mn.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ba.9csxet.cn

[Q27] 条件计数
来源：http://bm.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jo.shxzskj.cn

[Q28] 求和与平均
来源：http://oo.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vq.wgjwhj.cn

[Q29] 最大最小值
来源：http://pp.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oq.shtwfgs.cn

[Q30] 分组统计
来源：http://zi.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ur.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://um.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ha.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://qy.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lj.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cy.muxihuayi.cn

[Q33] 多列分组
来源：http://cr.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://er.haigaiapp.cn

[Q34] 每组取第一条
来源：http://np.colortex.cn

SELECT * FROM (
来源：http://ix.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aa.gzmigu.cn

) t WHERE rn = 1;
来源：http://pw.bjjhwx.cn

[Q35] 内连接
来源：http://wc.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://io.shtwfgs.cn

[Q36] 左连接
来源：http://fu.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ds.521024.cn

[Q37] 右连接
来源：http://xr.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aa.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yz.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://is.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://pj.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fe.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kw.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ig.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lp.jianghongdianzi.cn

[Q41] 多表连接
来源：http://ih.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ij.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://hz.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://ft.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://nd.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://kv.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ks.panjiajie.cn

[Q43] 标量子查询
来源：http://vd.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xa.nszjky.cn

[Q44] IN 子查询
来源：http://ng.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jf.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://pz.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rx.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ot.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pf.shtwfgs.cn

[Q47] 与平均值比较
来源：http://we.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://my.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://qy.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pu.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://oi.szsharing.cn

[Q49] 更新单行
来源：http://hq.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zo.bjjhwx.cn

[Q50] 批量更新
来源：http://uk.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hl.lnxyls.cn

[Q51] 用子查询更新
来源：http://iw.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nu.wgjwhj.cn

[Q52] 删除指定行
来源：http://tl.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://hd.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://hx.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gv.yuntaijiaju.cn

[Q54] 清空表
来源：http://dh.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://yo.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://ja.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sp.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://cz.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jr.newstarts.cn

[Q57] 行号
来源：http://fh.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cg.huixinmuqiang.cn

[Q58] 累计求和
来源：http://ym.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sz.chemitech.net.cn

[Q59] 分组内累计
来源：http://sp.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://or.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://nh.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yf.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zk.bjjhwx.cn

[Q61] 移动平均
来源：http://ud.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vl.yuexingan06.cn

[Q62] 分组占比
来源：http://de.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hj.wgjwhj.cn

[Q63] 开启事务
来源：http://rv.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nb.yuexingan06.cn

[Q64] 提交事务
来源：http://gl.jianghongdianzi.cn

COMMIT;
来源：http://er.gzmigu.cn

[Q65] 回滚事务
来源：http://qz.huanxung.cn

ROLLBACK;
来源：http://bz.jctech888.com.cn

[Q66] 行锁查询
来源：http://kg.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fm.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://zs.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qy.gzmigu.cn

[Q68] 保存点
来源：http://hh.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://iy.szxytkj.cn

ROLLBACK TO sp1;
来源：http://vl.shxzukj.cn

[Q69] 查看执行计划
来源：http://io.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bk.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://ji.bjjhwx.cn

ANALYZE TABLE users;
来源：http://oo.muxihuayi.cn

[Q71] 查看建表语句
来源：http://fy.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vm.nszjky.cn

[Q72] 查看索引
来源：http://jq.lnxyls.cn

SHOW INDEX FROM users;
来源：http://rb.bookmarksfly.cn

[Q73] 查看表状态
来源：http://qr.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://is.9csxet.cn

[Q74] 强制使用索引
来源：http://jl.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fd.szsharing.cn

[Q75] 日期格式化
来源：http://vw.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ac.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yz.colortex.cn


<!-- 参考信息 -->