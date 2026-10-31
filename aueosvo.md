代发 wailian999

================================================================================
来源：http://tr.jianghongdianzi.cn

O. 并发与异步
来源：http://gf.wgjwhj.cn

================================================================================
来源：http://it.wgjwhj.cn

[O01] 启动一个线程
来源：http://ez.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ah.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qs.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://za.colortex.cn

TS:   // 同 JS
来源：http://zo.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://xk.colortex.cn

Go:   go f()
来源：http://wz.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://vc.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ec.colortex.cn

[O02] 使用线程池
来源：http://ca.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wv.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ij.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://sj.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://iy.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://da.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wu.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://it.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://os.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://hb.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://wb.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ue.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fw.huixinmuqiang.cn

TS:   // 同 JS
来源：http://dw.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://jd.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fk.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bw.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://yb.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://wv.asd995.cn

Py:   async def f():⏎    await g()
来源：http://ni.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pr.asd995.cn

JS:   async function f() { await g(); }
来源：http://nv.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hc.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xp.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kl.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mz.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://uj.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://np.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://qz.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xs.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://fk.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://sm.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ks.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uq.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ix.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fp.yuntaijiaju.cn

[O06] 使用进程池
来源：http://wa.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://np.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qe.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://pj.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://yf.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fk.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nb.hnjuh.cn

Ruby: // fork 块
来源：http://pr.wgjwhj.cn

C#:   Parallel.For
来源：http://ye.shtwfgs.cn

================================================================================
来源：http://bn.jctech888.com.cn

P. 常用工具函数
来源：http://ad.hahajie.cn

================================================================================
来源：http://df.jctech888.com.cn

[P01] 生成 UUID
来源：http://cy.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://qs.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ro.hahajie.cn

JS:   crypto.randomUUID()
来源：http://ef.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://gl.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://oe.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://ps.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://fk.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://jc.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://dq.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gb.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://on.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://na.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://at.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vu.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lt.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://te.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pi.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://rn.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gc.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gx.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hb.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lk.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dr.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ff.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hg.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jk.yuntaijiaju.cn

[P04] 求长度
来源：http://ci.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cz.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ih.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zk.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ml.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://sf.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://xt.szxytkj.cn

Ruby: x.length;  x.size
来源：http://jt.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vy.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://fc.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dc.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wa.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ax.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tx.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ce.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://it.hnjuh.cn

Ruby: a == b
来源：http://od.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qi.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tp.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rm.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://it.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pq.nszjky.cn

TS:   if (x == null) {}
来源：http://rh.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sj.gzmigu.cn

Go:   if x == nil {}
来源：http://jh.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ij.muxihuayi.cn

C#:   if (x is null) {}
来源：http://kq.hnjuh.cn

[P07] 防抖与节流
来源：http://fz.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dv.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://rt.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hv.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mv.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ax.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gz.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ex.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ha.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://bb.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zg.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ua.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://re.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vg.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zx.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cv.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xf.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kp.bookmarksfly.cn

================================================================================
来源：http://pi.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ea.huixiangedu.cn

================================================================================
来源：http://zy.yuexingan06.cn

[Q01] 创建表
来源：http://fl.shxzskj.cn

CREATE TABLE users (
来源：http://ak.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cv.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://sg.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://ov.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lu.521024.cn

);
来源：http://kw.colortex.cn

[Q02] 创建带外键的表
来源：http://so.colortex.cn

CREATE TABLE orders (
来源：http://qw.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ru.gzmigu.cn

user_id INT NOT NULL,
来源：http://ki.colortex.cn

amount DECIMAL(10, 2),
来源：http://vm.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cf.gzmigu.cn

);
来源：http://sv.jianghongdianzi.cn

[Q03] 增加列
来源：http://tx.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://db.shxzskj.cn

[Q04] 修改列类型
来源：http://qy.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eq.wgjwhj.cn

[Q05] 重命名列
来源：http://fp.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ya.panjiajie.cn

[Q06] 删除列
来源：http://li.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lb.nszjky.cn

[Q07] 删除表
来源：http://bn.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://lf.nicolike.cn

[Q08] 创建普通索引
来源：http://jm.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fh.hnjuh.cn

[Q09] 创建唯一索引
来源：http://bx.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bz.muxihuayi.cn

[Q10] 插入单行
来源：http://ic.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vt.huixiangedu.cn

[Q11] 一次插入多行
来源：http://pk.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fj.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://tv.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nn.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://st.nicolike.cn

[Q13] 忽略重复插入
来源：http://ps.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hs.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://gq.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wq.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ia.521024.cn

[Q15] 查询全部
来源：http://hx.jianghongdianzi.cn

SELECT * FROM users;
来源：http://tu.hahajie.cn

[Q16] 查询指定列
来源：http://pr.lnxyls.cn

SELECT id, name FROM users;
来源：http://uo.521024.cn

[Q17] 条件查询
来源：http://ta.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qq.nszjky.cn

[Q18] 模糊匹配
来源：http://km.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nn.yuntaijiaju.cn

[Q19] 范围查询
来源：http://lf.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nq.9csxet.cn

[Q20] IN 列表
来源：http://vc.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eg.shtwfgs.cn

[Q21] 空值判断
来源：http://wr.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qh.chemitech.net.cn

[Q22] 排序
来源：http://pf.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cw.szsharing.cn

[Q23] 分页
来源：http://qo.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sd.lnxyls.cn

[Q24] 去重
来源：http://ud.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://os.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://gg.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qn.jianghongdianzi.cn

[Q26] 计数
来源：http://sc.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://ef.gzmigu.cn

[Q27] 条件计数
来源：http://sm.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zc.muxihuayi.cn

[Q28] 求和与平均
来源：http://xf.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yc.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://ug.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bk.muxihuayi.cn

[Q30] 分组统计
来源：http://zh.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wh.bjjhwx.cn

[Q31] 分组后过滤
来源：http://rb.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fq.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://zf.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cf.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lc.wgjwhj.cn

[Q33] 多列分组
来源：http://ub.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lz.nszjky.cn

[Q34] 每组取第一条
来源：http://ip.gzmigu.cn

SELECT * FROM (
来源：http://gc.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kt.haigaiapp.cn

) t WHERE rn = 1;
来源：http://kf.nszjky.cn

[Q35] 内连接
来源：http://or.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tk.newstarts.cn

[Q36] 左连接
来源：http://xy.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uf.szxytkj.cn

[Q37] 右连接
来源：http://vv.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xn.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zs.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qr.521024.cn

[Q39] 自连接（查上下级）
来源：http://jd.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vv.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fd.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hy.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gz.yuexingan06.cn

[Q41] 多表连接
来源：http://bp.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://do.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://xj.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://kv.colortex.cn

[Q42] 连接条件附加过滤
来源：http://az.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ev.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nb.wgjwhj.cn

[Q43] 标量子查询
来源：http://ck.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tb.newstarts.cn

[Q44] IN 子查询
来源：http://lg.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ph.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://fy.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iq.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pt.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iy.colortex.cn

[Q47] 与平均值比较
来源：http://xx.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uq.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://wn.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ga.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://xc.szsharing.cn

[Q49] 更新单行
来源：http://pl.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tp.lnxyls.cn

[Q50] 批量更新
来源：http://lv.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://np.shxzukj.cn

[Q51] 用子查询更新
来源：http://aq.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qz.bjjhwx.cn

[Q52] 删除指定行
来源：http://iu.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://ct.shtwfgs.cn

[Q53] 按条件删除
来源：http://qa.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ql.shxzukj.cn

[Q54] 清空表
来源：http://hh.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://cb.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://kd.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lx.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://pj.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ou.shtwfgs.cn

[Q57] 行号
来源：http://ws.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ok.szxytkj.cn

[Q58] 累计求和
来源：http://an.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://td.huixiangedu.cn

[Q59] 分组内累计
来源：http://kn.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://io.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://zn.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://da.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uo.asd995.cn

[Q61] 移动平均
来源：http://ig.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ne.huixinmuqiang.cn

[Q62] 分组占比
来源：http://qi.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vu.newstarts.cn

[Q63] 开启事务
来源：http://ja.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ap.bookmarksfly.cn

[Q64] 提交事务
来源：http://vs.shtwfgs.cn

COMMIT;
来源：http://ru.shxzskj.cn

[Q65] 回滚事务
来源：http://eh.shxzukj.cn

ROLLBACK;
来源：http://ck.9csxet.cn

[Q66] 行锁查询
来源：http://gh.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://el.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://ba.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ld.bjjhwx.cn

[Q68] 保存点
来源：http://ew.panjiajie.cn

SAVEPOINT sp1;
来源：http://fn.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://tn.yuexingan06.cn

[Q69] 查看执行计划
来源：http://wj.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jh.szxytkj.cn

[Q70] 更新统计信息
来源：http://pt.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://nh.muxihuayi.cn

[Q71] 查看建表语句
来源：http://ke.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uc.szxytkj.cn

[Q72] 查看索引
来源：http://po.szxytkj.cn


<!-- 参考信息 -->