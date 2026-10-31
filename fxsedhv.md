代发 wailian999

================================================================================
来源：http://cr.szxytkj.cn

O. 并发与异步
来源：http://nx.haigaiapp.cn

================================================================================
来源：http://et.nszjky.cn

[O01] 启动一个线程
来源：http://xb.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sb.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hm.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://de.wgjwhj.cn

TS:   // 同 JS
来源：http://pd.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://ck.panjiajie.cn

Go:   go f()
来源：http://sg.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ap.asd995.cn

C#:   Task.Run(() => F());
来源：http://ol.huixinmuqiang.cn

[O02] 使用线程池
来源：http://xh.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tq.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sc.9csxet.cn

JS:   // worker_threads 线程池
来源：http://vw.hahajie.cn

TS:   // worker_threads 线程池
来源：http://vj.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oz.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wx.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ur.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nk.521024.cn

[O03] 加锁保护共享数据
来源：http://jp.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://zq.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://aa.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xq.newstarts.cn

TS:   // 同 JS
来源：http://oi.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://gs.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rv.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cx.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://ax.hahajie.cn

[O04] 定义异步函数并等待
来源：http://ts.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://lu.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ua.9csxet.cn

JS:   async function f() { await g(); }
来源：http://nn.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://px.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rp.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iq.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hr.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://id.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://ur.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://mu.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qm.colortex.cn

JS:   await Promise.all(tasks)
来源：http://py.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ki.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zc.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mz.9csxet.cn

Ruby: threads.map(&:join)
来源：http://hv.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nn.bjjhwx.cn

[O06] 使用进程池
来源：http://hp.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dm.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ub.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://yk.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://pq.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xx.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tk.jianghongdianzi.cn

Ruby: // fork 块
来源：http://pe.nszjky.cn

C#:   Parallel.For
来源：http://vn.szsharing.cn

================================================================================
来源：http://xz.bjjhwx.cn

P. 常用工具函数
来源：http://ss.shxzskj.cn

================================================================================
来源：http://fb.hahajie.cn

[P01] 生成 UUID
来源：http://if.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://fv.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ar.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://vc.521024.cn

TS:   crypto.randomUUID()
来源：http://vt.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://go.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://ao.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://fx.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ir.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://rj.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uv.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lx.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://me.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://md.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sq.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zk.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ah.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pu.gzmigu.cn

[P03] 生成短随机字符串
来源：http://om.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ea.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ja.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hq.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gg.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rj.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ap.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gi.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yl.lnxyls.cn

[P04] 求长度
来源：http://lv.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sz.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eu.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kl.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qn.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://eu.huanxung.cn

Go:   len(arr);  len(m)
来源：http://eq.shxzukj.cn

Ruby: x.length;  x.size
来源：http://to.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zx.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://jm.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ky.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yb.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jj.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yy.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kq.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kg.newstarts.cn

Ruby: a == b
来源：http://kb.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kc.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tq.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rr.colortex.cn

PHP:  if (empty($x)) {}
来源：http://tl.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ge.521024.cn

TS:   if (x == null) {}
来源：http://ur.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uh.hahajie.cn

Go:   if x == nil {}
来源：http://wj.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bq.nszjky.cn

C#:   if (x is null) {}
来源：http://tz.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://dh.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fa.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://jf.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ux.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kl.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fy.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lt.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ju.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ki.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://pr.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uk.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ci.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zi.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nr.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tf.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qz.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oz.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sw.haigaiapp.cn

================================================================================
来源：http://ys.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wk.chemitech.net.cn

================================================================================
来源：http://wn.shxzskj.cn

[Q01] 创建表
来源：http://zv.shtwfgs.cn

CREATE TABLE users (
来源：http://bz.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ld.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://ky.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://sq.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yw.gzmigu.cn

);
来源：http://xo.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://wl.huanxung.cn

CREATE TABLE orders (
来源：http://em.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sp.hnjuh.cn

user_id INT NOT NULL,
来源：http://lh.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://nf.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zn.bjjhwx.cn

);
来源：http://hk.huixinmuqiang.cn

[Q03] 增加列
来源：http://ue.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ct.shxzukj.cn

[Q04] 修改列类型
来源：http://nu.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gr.bjjhwx.cn

[Q05] 重命名列
来源：http://je.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ut.huixinmuqiang.cn

[Q06] 删除列
来源：http://sa.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://co.haigaiapp.cn

[Q07] 删除表
来源：http://vm.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://os.asd995.cn

[Q08] 创建普通索引
来源：http://nb.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ol.9csxet.cn

[Q09] 创建唯一索引
来源：http://so.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ip.shxzukj.cn

[Q10] 插入单行
来源：http://xs.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fc.hnjuh.cn

[Q11] 一次插入多行
来源：http://kn.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nn.colortex.cn

[Q12] 插入后取自增 ID
来源：http://gp.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qw.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tb.shxzskj.cn

[Q13] 忽略重复插入
来源：http://bx.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sw.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://gt.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tt.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://is.bjjhwx.cn

[Q15] 查询全部
来源：http://qn.lnxyls.cn

SELECT * FROM users;
来源：http://ew.yuexingan06.cn

[Q16] 查询指定列
来源：http://zu.jctech888.com.cn

SELECT id, name FROM users;
来源：http://qt.shxzskj.cn

[Q17] 条件查询
来源：http://yd.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bf.yuexingan06.cn

[Q18] 模糊匹配
来源：http://bm.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yc.newstarts.cn

[Q19] 范围查询
来源：http://xa.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pm.lnxyls.cn

[Q20] IN 列表
来源：http://iw.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wv.yuexingan06.cn

[Q21] 空值判断
来源：http://nf.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vt.haigaiapp.cn

[Q22] 排序
来源：http://ks.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ve.szsharing.cn

[Q23] 分页
来源：http://tf.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ee.nszjky.cn

[Q24] 去重
来源：http://mg.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://zw.panjiajie.cn

[Q25] 只取前 N 条
来源：http://dk.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dp.colortex.cn

[Q26] 计数
来源：http://tj.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://nu.521024.cn

[Q27] 条件计数
来源：http://ad.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xz.521024.cn

[Q28] 求和与平均
来源：http://xa.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jb.huixiangedu.cn

[Q29] 最大最小值
来源：http://mr.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://he.huanxung.cn

[Q30] 分组统计
来源：http://uo.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ws.newstarts.cn

[Q31] 分组后过滤
来源：http://ji.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jk.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://gj.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pg.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yn.521024.cn

[Q33] 多列分组
来源：http://gr.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ga.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://jd.lnxyls.cn

SELECT * FROM (
来源：http://cj.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wf.asd995.cn

) t WHERE rn = 1;
来源：http://dm.huixinmuqiang.cn

[Q35] 内连接
来源：http://gc.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bv.bjjhwx.cn

[Q36] 左连接
来源：http://ps.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://we.gzmigu.cn

[Q37] 右连接
来源：http://eo.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pb.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fx.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://un.colortex.cn

[Q39] 自连接（查上下级）
来源：http://rk.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dd.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uz.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bl.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hl.jianghongdianzi.cn

[Q41] 多表连接
来源：http://ha.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qu.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://yz.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://rt.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://yy.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://xt.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qy.521024.cn

[Q43] 标量子查询
来源：http://sd.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ra.huixiangedu.cn

[Q44] IN 子查询
来源：http://ro.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qv.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://eu.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vb.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vv.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xe.521024.cn

[Q47] 与平均值比较
来源：http://ec.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pt.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ss.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vl.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://qh.yuexingan06.cn

[Q49] 更新单行
来源：http://gn.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://au.colortex.cn

[Q50] 批量更新
来源：http://pm.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ze.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://fs.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://il.szsharing.cn

[Q52] 删除指定行
来源：http://pk.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://la.huixiangedu.cn

[Q53] 按条件删除
来源：http://fq.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fo.panjiajie.cn

[Q54] 清空表
来源：http://tj.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://ye.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://bw.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ys.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://lk.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xo.nicolike.cn

[Q57] 行号
来源：http://cy.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://li.shxzukj.cn

[Q58] 累计求和
来源：http://ds.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wc.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://ev.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ob.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://ol.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xg.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ur.bjjhwx.cn

[Q61] 移动平均
来源：http://pp.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sy.gzmigu.cn

[Q62] 分组占比
来源：http://kp.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jk.bookmarksfly.cn

[Q63] 开启事务
来源：http://gm.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gd.nszjky.cn

[Q64] 提交事务
来源：http://im.wgjwhj.cn

COMMIT;
来源：http://vb.wgjwhj.cn

[Q65] 回滚事务
来源：http://cz.muxihuayi.cn

ROLLBACK;
来源：http://vs.chemitech.net.cn

[Q66] 行锁查询
来源：http://zy.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bz.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://sc.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kj.yuntaijiaju.cn

[Q68] 保存点
来源：http://my.shtwfgs.cn

SAVEPOINT sp1;
来源：http://bq.521024.cn

ROLLBACK TO sp1;
来源：http://zk.colortex.cn

[Q69] 查看执行计划
来源：http://xj.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cp.chemitech.net.cn

[Q70] 更新统计信息
来源：http://wg.panjiajie.cn

ANALYZE TABLE users;
来源：http://hp.9csxet.cn

[Q71] 查看建表语句
来源：http://dz.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eb.huixiangedu.cn

[Q72] 查看索引
来源：http://sk.huixiangedu.cn


<!-- 参考信息 -->