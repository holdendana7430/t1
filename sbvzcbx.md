代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://ii.yuexingan06.cn

Go:   go f()
来源：http://bd.szxytkj.cn

Ruby: Thread.new { f }
来源：http://zu.nszjky.cn

C#:   Task.Run(() => F());
来源：http://pa.jctech888.com.cn

[O02] 使用线程池
来源：http://sq.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lh.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eg.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://fe.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://qw.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qa.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xa.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xj.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pa.colortex.cn

[O03] 加锁保护共享数据
来源：http://rw.hahajie.cn

Py:   with lock: shared += 1
来源：http://hm.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://pq.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kb.wgjwhj.cn

TS:   // 同 JS
来源：http://lz.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://eh.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hu.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cg.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://xx.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://tz.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ci.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ka.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://in.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bz.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nd.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kg.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hz.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://lt.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://zd.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://tg.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uw.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://me.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://zx.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fl.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xd.521024.cn

Ruby: threads.map(&:join)
来源：http://xf.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zt.huixiangedu.cn

[O06] 使用进程池
来源：http://ck.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mq.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kf.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://hs.asd995.cn

TS:   // child_process / cluster 模块
来源：http://jm.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zo.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ec.9csxet.cn

Ruby: // fork 块
来源：http://zs.shtwfgs.cn

C#:   Parallel.For
来源：http://xe.jianghongdianzi.cn

================================================================================
来源：http://yz.shxzukj.cn

P. 常用工具函数
来源：http://kp.wgjwhj.cn

================================================================================
来源：http://rb.szsharing.cn

[P01] 生成 UUID
来源：http://ri.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://tv.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wb.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://ei.colortex.cn

TS:   crypto.randomUUID()
来源：http://jz.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://gz.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://fe.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://fa.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://cv.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://ia.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dh.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nz.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ue.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wn.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://na.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pn.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pz.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vk.521024.cn

[P03] 生成短随机字符串
来源：http://ov.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://io.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jt.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://on.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lo.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xi.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jj.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://my.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lh.yuexingan06.cn

[P04] 求长度
来源：http://sa.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iv.huixinmuqiang.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aj.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qi.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://al.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://hd.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://rq.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ff.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rg.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://wy.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kl.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bw.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tn.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ii.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qa.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ty.huixiangedu.cn

Ruby: a == b
来源：http://zi.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oo.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nl.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jw.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ct.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jk.hahajie.cn

TS:   if (x == null) {}
来源：http://ua.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wn.newstarts.cn

Go:   if x == nil {}
来源：http://mn.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://in.szsharing.cn

C#:   if (x is null) {}
来源：http://cz.asd995.cn

[P07] 防抖与节流
来源：http://qo.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ti.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://of.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ud.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ad.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jm.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ys.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nd.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uv.asd995.cn

[P08] 处理浮点精度问题
来源：http://dj.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oy.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://te.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uy.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ji.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ft.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ts.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zy.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ny.szsharing.cn

================================================================================
来源：http://au.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ik.shxzskj.cn

================================================================================
来源：http://hp.bjjhwx.cn

[Q01] 创建表
来源：http://qi.9csxet.cn

CREATE TABLE users (
来源：http://nv.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lk.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://ea.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://jm.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bt.huixinmuqiang.cn

);
来源：http://qp.nszjky.cn

[Q02] 创建带外键的表
来源：http://bd.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://wc.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wk.bjjhwx.cn

user_id INT NOT NULL,
来源：http://bl.newstarts.cn

amount DECIMAL(10, 2),
来源：http://si.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qh.asd995.cn

);
来源：http://ai.huixinmuqiang.cn

[Q03] 增加列
来源：http://hi.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ia.colortex.cn

[Q04] 修改列类型
来源：http://qi.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sb.521024.cn

[Q05] 重命名列
来源：http://fj.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jn.hnjuh.cn

[Q06] 删除列
来源：http://tl.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bx.bjjhwx.cn

[Q07] 删除表
来源：http://pe.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://zu.panjiajie.cn

[Q08] 创建普通索引
来源：http://kg.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zk.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://au.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cf.yuexingan06.cn

[Q10] 插入单行
来源：http://ks.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mn.haigaiapp.cn

[Q11] 一次插入多行
来源：http://ik.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ug.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://bn.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lg.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qf.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://qn.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dq.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://io.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://om.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://io.yuntaijiaju.cn

[Q15] 查询全部
来源：http://il.panjiajie.cn

SELECT * FROM users;
来源：http://mh.lnxyls.cn

[Q16] 查询指定列
来源：http://un.shxzskj.cn

SELECT id, name FROM users;
来源：http://jr.nicolike.cn

[Q17] 条件查询
来源：http://pn.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qa.hahajie.cn

[Q18] 模糊匹配
来源：http://ca.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vg.nszjky.cn

[Q19] 范围查询
来源：http://lt.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sx.nszjky.cn

[Q20] IN 列表
来源：http://ke.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sa.lnxyls.cn

[Q21] 空值判断
来源：http://gv.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hahajie.cn

[Q22] 排序
来源：http://va.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vm.hnjuh.cn

[Q23] 分页
来源：http://tb.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ox.chemitech.net.cn

[Q24] 去重
来源：http://by.521024.cn

SELECT DISTINCT city FROM users;
来源：http://rg.colortex.cn

[Q25] 只取前 N 条
来源：http://oy.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://re.muxihuayi.cn

[Q26] 计数
来源：http://dg.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://sc.nicolike.cn

[Q27] 条件计数
来源：http://yh.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ao.chemitech.net.cn

[Q28] 求和与平均
来源：http://qy.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ah.nszjky.cn

[Q29] 最大最小值
来源：http://ae.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ne.newstarts.cn

[Q30] 分组统计
来源：http://cg.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sh.wgjwhj.cn

[Q31] 分组后过滤
来源：http://pb.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rh.nszjky.cn

[Q32] 分组拼接字符串
来源：http://zp.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bq.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bq.nszjky.cn

[Q33] 多列分组
来源：http://iz.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dr.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://aw.jctech888.com.cn

SELECT * FROM (
来源：http://lb.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://py.huanxung.cn

) t WHERE rn = 1;
来源：http://ap.shxzukj.cn

[Q35] 内连接
来源：http://up.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mf.lnxyls.cn

[Q36] 左连接
来源：http://hq.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ss.hahajie.cn

[Q37] 右连接
来源：http://lb.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ka.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gt.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qa.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://br.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iz.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cl.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lc.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mi.muxihuayi.cn

[Q41] 多表连接
来源：http://qf.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pf.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://kx.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://kl.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://us.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://ae.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zk.szsharing.cn

[Q43] 标量子查询
来源：http://ny.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://he.colortex.cn

[Q44] IN 子查询
来源：http://bw.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dx.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://xk.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wz.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ub.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rs.wgjwhj.cn

[Q47] 与平均值比较
来源：http://un.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rb.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://aw.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ep.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://ay.lnxyls.cn

[Q49] 更新单行
来源：http://wn.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uo.huanxung.cn

[Q50] 批量更新
来源：http://do.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oc.colortex.cn

[Q51] 用子查询更新
来源：http://nv.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hx.szsharing.cn

[Q52] 删除指定行
来源：http://yj.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://lg.colortex.cn

[Q53] 按条件删除
来源：http://ok.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vy.shtwfgs.cn

[Q54] 清空表
来源：http://bn.hahajie.cn

TRUNCATE TABLE logs;
来源：http://jz.newstarts.cn

[Q55] 排名（并列占位）
来源：http://va.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mr.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://wz.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://av.yuntaijiaju.cn

[Q57] 行号
来源：http://oj.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yx.bjjhwx.cn

[Q58] 累计求和
来源：http://qn.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cs.shxzukj.cn

[Q59] 分组内累计
来源：http://am.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zo.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://vs.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jb.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bs.hnjuh.cn

[Q61] 移动平均
来源：http://df.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ga.jctech888.com.cn

[Q62] 分组占比
来源：http://lv.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nl.szsharing.cn

[Q63] 开启事务
来源：http://kd.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tz.shtwfgs.cn

[Q64] 提交事务
来源：http://ys.hnjuh.cn

COMMIT;
来源：http://ua.szxytkj.cn

[Q65] 回滚事务
来源：http://zg.hnjuh.cn

ROLLBACK;
来源：http://yx.muxihuayi.cn

[Q66] 行锁查询
来源：http://wc.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sl.shxzukj.cn

[Q67] 设置隔离级别
来源：http://qr.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ie.chemitech.net.cn

[Q68] 保存点
来源：http://vo.9csxet.cn

SAVEPOINT sp1;
来源：http://uq.hahajie.cn

ROLLBACK TO sp1;
来源：http://mt.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://hn.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zf.hnjuh.cn

[Q70] 更新统计信息
来源：http://av.nicolike.cn

ANALYZE TABLE users;
来源：http://ax.jctech888.com.cn

[Q71] 查看建表语句
来源：http://rt.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sx.jianghongdianzi.cn

[Q72] 查看索引
来源：http://ed.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://ct.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://fe.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ym.9csxet.cn

[Q74] 强制使用索引
来源：http://bb.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zz.shxzskj.cn

[Q75] 日期格式化
来源：http://qc.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yp.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mp.newstarts.cn


<!-- 参考信息 -->