代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mf.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ai.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fb.bjjhwx.cn

TS:   // 同 JS
来源：http://lr.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://ds.gzmigu.cn

Go:   go f()
来源：http://kx.panjiajie.cn

Ruby: Thread.new { f }
来源：http://oy.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://sn.haigaiapp.cn

[O02] 使用线程池
来源：http://xx.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xh.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wi.9csxet.cn

JS:   // worker_threads 线程池
来源：http://um.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://ox.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sy.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qm.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xq.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zf.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://sp.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://rg.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://jk.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vu.huixiangedu.cn

TS:   // 同 JS
来源：http://lh.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://xu.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://me.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lw.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://pr.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ai.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://nf.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kh.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://qq.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://do.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oy.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dw.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kp.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://xr.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://tj.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://dq.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qc.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://mr.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://hv.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ns.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nx.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://tf.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hp.wgjwhj.cn

[O06] 使用进程池
来源：http://iw.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xu.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ln.521024.cn

JS:   // child_process / cluster 模块
来源：http://tv.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ij.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ow.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vq.colortex.cn

Ruby: // fork 块
来源：http://nm.colortex.cn

C#:   Parallel.For
来源：http://hl.haigaiapp.cn

================================================================================
来源：http://ce.muxihuayi.cn

P. 常用工具函数
来源：http://gq.521024.cn

================================================================================
来源：http://vg.bookmarksfly.cn

[P01] 生成 UUID
来源：http://bx.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://le.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ym.521024.cn

JS:   crypto.randomUUID()
来源：http://qn.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://ih.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://sc.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://jm.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://xw.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://dm.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://qs.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tk.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kc.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vq.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qk.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dt.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ek.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bu.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pg.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://zi.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yl.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xm.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bc.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dr.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ou.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vx.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jo.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oj.gzmigu.cn

[P04] 求长度
来源：http://dd.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fr.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vw.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kj.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://nz.nszjky.cn

Go:   len(arr);  len(m)
来源：http://qk.nszjky.cn

Ruby: x.length;  x.size
来源：http://hn.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://us.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://yg.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://br.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zk.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://in.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pe.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vf.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xo.bjjhwx.cn

Ruby: a == b
来源：http://ep.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yg.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yu.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dp.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://mh.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gf.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ty.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hs.gzmigu.cn

Go:   if x == nil {}
来源：http://dr.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tn.521024.cn

C#:   if (x is null) {}
来源：http://mz.hahajie.cn

[P07] 防抖与节流
来源：http://cd.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://te.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://ex.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mc.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vf.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ye.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://to.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gl.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hw.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://ol.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zz.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jw.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lt.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hp.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://km.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://na.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ot.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ia.colortex.cn

================================================================================
来源：http://pq.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ao.asd995.cn

================================================================================
来源：http://km.gzmigu.cn

[Q01] 创建表
来源：http://yp.huixiangedu.cn

CREATE TABLE users (
来源：http://rq.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ct.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://ec.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://if.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ss.nszjky.cn

);
来源：http://vk.panjiajie.cn

[Q02] 创建带外键的表
来源：http://es.colortex.cn

CREATE TABLE orders (
来源：http://jx.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ag.521024.cn

user_id INT NOT NULL,
来源：http://nk.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://mn.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fv.huixinmuqiang.cn

);
来源：http://mr.shtwfgs.cn

[Q03] 增加列
来源：http://oh.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hx.shtwfgs.cn

[Q04] 修改列类型
来源：http://bq.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ie.asd995.cn

[Q05] 重命名列
来源：http://lz.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yx.521024.cn

[Q06] 删除列
来源：http://yi.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ev.hnjuh.cn

[Q07] 删除表
来源：http://gm.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://bl.shxzukj.cn

[Q08] 创建普通索引
来源：http://os.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gp.huanxung.cn

[Q09] 创建唯一索引
来源：http://cf.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ol.shxzskj.cn

[Q10] 插入单行
来源：http://zz.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hs.521024.cn

[Q11] 一次插入多行
来源：http://mc.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lo.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://bp.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mw.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hi.521024.cn

[Q13] 忽略重复插入
来源：http://pj.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kh.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://fb.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hk.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rf.chemitech.net.cn

[Q15] 查询全部
来源：http://vx.yuexingan06.cn

SELECT * FROM users;
来源：http://zb.szxytkj.cn

[Q16] 查询指定列
来源：http://jv.hnjuh.cn

SELECT id, name FROM users;
来源：http://yc.wgjwhj.cn

[Q17] 条件查询
来源：http://jy.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ia.jctech888.com.cn

[Q18] 模糊匹配
来源：http://wb.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kw.shxzskj.cn

[Q19] 范围查询
来源：http://ok.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jz.wgjwhj.cn

[Q20] IN 列表
来源：http://nr.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iy.wgjwhj.cn

[Q21] 空值判断
来源：http://ft.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mn.shxzskj.cn

[Q22] 排序
来源：http://lh.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zw.huixinmuqiang.cn

[Q23] 分页
来源：http://zj.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xm.nicolike.cn

[Q24] 去重
来源：http://he.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://ea.hnjuh.cn

[Q25] 只取前 N 条
来源：http://ks.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://az.9csxet.cn

[Q26] 计数
来源：http://mp.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://np.szsharing.cn

[Q27] 条件计数
来源：http://eu.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ub.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://ke.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://so.nszjky.cn

[Q29] 最大最小值
来源：http://kg.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iv.huixinmuqiang.cn

[Q30] 分组统计
来源：http://st.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ar.colortex.cn

[Q31] 分组后过滤
来源：http://rz.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xr.nicolike.cn

[Q32] 分组拼接字符串
来源：http://cg.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ge.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zk.newstarts.cn

[Q33] 多列分组
来源：http://ja.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lr.shxzskj.cn

[Q34] 每组取第一条
来源：http://lw.panjiajie.cn

SELECT * FROM (
来源：http://hn.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ep.shxzukj.cn

) t WHERE rn = 1;
来源：http://xt.521024.cn

[Q35] 内连接
来源：http://or.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vr.chemitech.net.cn

[Q36] 左连接
来源：http://iw.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ju.shtwfgs.cn

[Q37] 右连接
来源：http://vo.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vd.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vz.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pg.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://op.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ff.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qo.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pb.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mu.muxihuayi.cn

[Q41] 多表连接
来源：http://bh.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ne.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://xa.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://ki.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://uy.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://pz.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ob.bjjhwx.cn

[Q43] 标量子查询
来源：http://fe.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ie.nicolike.cn

[Q44] IN 子查询
来源：http://ts.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zr.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://gq.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pn.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://un.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hv.hahajie.cn

[Q47] 与平均值比较
来源：http://dh.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qk.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://js.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bt.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://tz.wgjwhj.cn

[Q49] 更新单行
来源：http://hq.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qz.lnxyls.cn

[Q50] 批量更新
来源：http://hp.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qm.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://qs.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gz.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://va.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://ot.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://wl.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ys.nicolike.cn

[Q54] 清空表
来源：http://tk.asd995.cn

TRUNCATE TABLE logs;
来源：http://vl.hahajie.cn

[Q55] 排名（并列占位）
来源：http://jr.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://my.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://tn.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tw.huixiangedu.cn

[Q57] 行号
来源：http://vy.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gl.huanxung.cn

[Q58] 累计求和
来源：http://jr.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dp.bookmarksfly.cn

[Q59] 分组内累计
来源：http://vg.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xe.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://ab.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bx.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dc.9csxet.cn

[Q61] 移动平均
来源：http://fv.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gu.shxzskj.cn

[Q62] 分组占比
来源：http://pu.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ic.bookmarksfly.cn

[Q63] 开启事务
来源：http://ag.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ie.shxzskj.cn

[Q64] 提交事务
来源：http://xt.bjjhwx.cn

COMMIT;
来源：http://np.hnjuh.cn

[Q65] 回滚事务
来源：http://wd.shxzukj.cn

ROLLBACK;
来源：http://hh.huanxung.cn

[Q66] 行锁查询
来源：http://zg.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qy.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://qv.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ch.bjjhwx.cn

[Q68] 保存点
来源：http://ns.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://vi.lnxyls.cn

ROLLBACK TO sp1;
来源：http://hf.bjjhwx.cn

[Q69] 查看执行计划
来源：http://hu.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vm.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://zq.szsharing.cn

ANALYZE TABLE users;
来源：http://st.szxytkj.cn

[Q71] 查看建表语句
来源：http://ps.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://us.huixiangedu.cn

[Q72] 查看索引
来源：http://bf.hahajie.cn

SHOW INDEX FROM users;
来源：http://eg.wgjwhj.cn

[Q73] 查看表状态
来源：http://xh.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zd.panjiajie.cn

[Q74] 强制使用索引
来源：http://gt.jctech888.com.cn


<!-- 参考信息 -->