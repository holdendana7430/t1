代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://ee.yuntaijiaju.cn

Go:   go f()
来源：http://sr.521024.cn

Ruby: Thread.new { f }
来源：http://xe.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://yl.9csxet.cn

[O02] 使用线程池
来源：http://wn.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ud.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nx.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://nn.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://op.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://az.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dm.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://on.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mh.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://uj.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://sg.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://ye.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rb.szxytkj.cn

TS:   // 同 JS
来源：http://ch.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://qy.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uw.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oo.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://gz.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://nj.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://vi.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://az.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://sk.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uf.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ey.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qs.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tl.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://ee.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://yd.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://gr.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ca.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://ya.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://pf.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ac.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ml.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://dz.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vv.9csxet.cn

[O06] 使用进程池
来源：http://ms.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ja.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jg.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://fl.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://sa.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uf.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uh.lnxyls.cn

Ruby: // fork 块
来源：http://xt.newstarts.cn

C#:   Parallel.For
来源：http://wc.szsharing.cn

================================================================================
来源：http://vm.bjjhwx.cn

P. 常用工具函数
来源：http://sy.haigaiapp.cn

================================================================================
来源：http://he.nicolike.cn

[P01] 生成 UUID
来源：http://md.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://nv.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sk.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://ca.huanxung.cn

TS:   crypto.randomUUID()
来源：http://cv.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://ju.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://hh.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://as.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://fa.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://ai.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wp.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cl.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gp.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xw.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wl.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hq.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sk.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kn.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://fv.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mv.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hf.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ze.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oh.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://in.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://na.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yx.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fv.newstarts.cn

[P04] 求长度
来源：http://ll.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ht.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nc.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nd.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ux.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://ps.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ix.colortex.cn

Ruby: x.length;  x.size
来源：http://cf.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jr.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://fj.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://li.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yp.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qt.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ku.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tk.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nv.panjiajie.cn

Ruby: a == b
来源：http://cf.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qf.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://go.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ji.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://md.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dd.nicolike.cn

TS:   if (x == null) {}
来源：http://cw.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tr.jctech888.com.cn

Go:   if x == nil {}
来源：http://hv.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tm.huanxung.cn

C#:   if (x is null) {}
来源：http://xm.newstarts.cn

[P07] 防抖与节流
来源：http://kx.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jr.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ns.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wj.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cw.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://td.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bb.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ht.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jo.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://ro.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pa.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rx.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hx.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nh.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bb.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ck.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://do.gzmigu.cn

================================================================================
来源：http://zn.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bl.9csxet.cn

================================================================================
来源：http://pw.bjjhwx.cn

[Q01] 创建表
来源：http://to.yuntaijiaju.cn

CREATE TABLE users (
来源：http://jm.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kr.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://fu.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://of.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ei.huixiangedu.cn

);
来源：http://xb.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://fl.yuexingan06.cn

CREATE TABLE orders (
来源：http://bk.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://km.bjjhwx.cn

user_id INT NOT NULL,
来源：http://zc.asd995.cn

amount DECIMAL(10, 2),
来源：http://ot.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ux.bookmarksfly.cn

);
来源：http://hu.haigaiapp.cn

[Q03] 增加列
来源：http://yy.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tz.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://gk.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ot.jianghongdianzi.cn

[Q05] 重命名列
来源：http://bt.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jd.asd995.cn

[Q06] 删除列
来源：http://uk.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ky.lnxyls.cn

[Q07] 删除表
来源：http://bz.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://or.asd995.cn

[Q08] 创建普通索引
来源：http://lv.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ns.newstarts.cn

[Q09] 创建唯一索引
来源：http://hq.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vt.bookmarksfly.cn

[Q10] 插入单行
来源：http://eo.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ti.chemitech.net.cn

[Q11] 一次插入多行
来源：http://tq.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ax.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://qs.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ui.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wa.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://ob.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ll.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://bx.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hx.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tc.shxzukj.cn

[Q15] 查询全部
来源：http://dy.bookmarksfly.cn

SELECT * FROM users;
来源：http://rs.shxzskj.cn

[Q16] 查询指定列
来源：http://dm.jctech888.com.cn

SELECT id, name FROM users;
来源：http://vj.nicolike.cn

[Q17] 条件查询
来源：http://iz.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://th.9csxet.cn

[Q18] 模糊匹配
来源：http://gk.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kq.9csxet.cn

[Q19] 范围查询
来源：http://gb.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ks.huanxung.cn

[Q20] IN 列表
来源：http://nl.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wz.asd995.cn

[Q21] 空值判断
来源：http://vt.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zx.szxytkj.cn

[Q22] 排序
来源：http://gd.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qg.shxzskj.cn

[Q23] 分页
来源：http://ha.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kz.bookmarksfly.cn

[Q24] 去重
来源：http://mj.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://bu.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://me.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ja.hahajie.cn

[Q26] 计数
来源：http://iw.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://hd.9csxet.cn

[Q27] 条件计数
来源：http://he.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wh.shtwfgs.cn

[Q28] 求和与平均
来源：http://cs.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mc.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://sv.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sv.chemitech.net.cn

[Q30] 分组统计
来源：http://ar.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sw.hnjuh.cn

[Q31] 分组后过滤
来源：http://nu.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dt.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://dp.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hk.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zw.newstarts.cn

[Q33] 多列分组
来源：http://qn.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lz.asd995.cn

[Q34] 每组取第一条
来源：http://mi.nszjky.cn

SELECT * FROM (
来源：http://tx.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://my.huixiangedu.cn

) t WHERE rn = 1;
来源：http://ug.shxzskj.cn

[Q35] 内连接
来源：http://yn.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ff.yuntaijiaju.cn

[Q36] 左连接
来源：http://zo.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uv.9csxet.cn

[Q37] 右连接
来源：http://by.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://en.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dk.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ky.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://sm.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pt.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zl.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xs.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kp.521024.cn

[Q41] 多表连接
来源：http://uw.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ep.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://lr.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ei.colortex.cn

[Q42] 连接条件附加过滤
来源：http://ov.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://br.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ue.muxihuayi.cn

[Q43] 标量子查询
来源：http://hi.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ws.bookmarksfly.cn

[Q44] IN 子查询
来源：http://wg.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ua.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://wy.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zj.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ig.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oq.colortex.cn

[Q47] 与平均值比较
来源：http://ed.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dj.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://fi.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hi.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://so.panjiajie.cn

[Q49] 更新单行
来源：http://eu.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dt.szsharing.cn

[Q50] 批量更新
来源：http://un.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vb.panjiajie.cn

[Q51] 用子查询更新
来源：http://vy.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://co.chemitech.net.cn

[Q52] 删除指定行
来源：http://ch.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://vc.yuexingan06.cn

[Q53] 按条件删除
来源：http://zb.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wz.panjiajie.cn

[Q54] 清空表
来源：http://kd.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://uj.521024.cn

[Q55] 排名（并列占位）
来源：http://yk.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://go.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://dy.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mu.shxzskj.cn

[Q57] 行号
来源：http://ru.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ei.yuexingan06.cn

[Q58] 累计求和
来源：http://gh.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jc.hnjuh.cn

[Q59] 分组内累计
来源：http://sf.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ur.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://fl.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bt.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://na.panjiajie.cn

[Q61] 移动平均
来源：http://wy.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nx.521024.cn

[Q62] 分组占比
来源：http://dj.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cj.hnjuh.cn

[Q63] 开启事务
来源：http://tg.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vd.gzmigu.cn

[Q64] 提交事务
来源：http://dz.shxzukj.cn

COMMIT;
来源：http://ee.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://hr.szsharing.cn

ROLLBACK;
来源：http://qs.jctech888.com.cn

[Q66] 行锁查询
来源：http://iy.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kv.nszjky.cn

[Q67] 设置隔离级别
来源：http://xg.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xs.panjiajie.cn

[Q68] 保存点
来源：http://hw.hnjuh.cn

SAVEPOINT sp1;
来源：http://gw.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://yh.9csxet.cn

[Q69] 查看执行计划
来源：http://wa.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fd.lnxyls.cn

[Q70] 更新统计信息
来源：http://ec.panjiajie.cn

ANALYZE TABLE users;
来源：http://de.nicolike.cn

[Q71] 查看建表语句
来源：http://js.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uv.gzmigu.cn

[Q72] 查看索引
来源：http://ba.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://cz.chemitech.net.cn

[Q73] 查看表状态
来源：http://vy.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fe.huixiangedu.cn

[Q74] 强制使用索引
来源：http://ug.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://os.jctech888.com.cn

[Q75] 日期格式化
来源：http://lm.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dd.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ym.huixiangedu.cn


<!-- 参考信息 -->