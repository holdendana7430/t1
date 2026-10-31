代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://jm.9csxet.cn

Go:   go f()
来源：http://xo.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://wl.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://qe.wgjwhj.cn

[O02] 使用线程池
来源：http://mb.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bm.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dr.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://ro.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://yi.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://za.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ls.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eq.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cz.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ky.521024.cn

Py:   with lock: shared += 1
来源：http://cl.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ax.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fg.hnjuh.cn

TS:   // 同 JS
来源：http://le.521024.cn

Java: synchronized (this) { shared++; }
来源：http://to.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tm.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nv.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://uo.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://yf.colortex.cn

Py:   async def f():⏎    await g()
来源：http://km.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cb.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://wl.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://di.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uk.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://em.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rx.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://qx.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://qp.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://pj.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dg.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://ys.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://qg.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pp.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ty.521024.cn

Ruby: threads.map(&:join)
来源：http://dx.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ru.shtwfgs.cn

[O06] 使用进程池
来源：http://ug.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ij.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rh.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://rs.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://ug.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lg.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pr.shxzskj.cn

Ruby: // fork 块
来源：http://kv.newstarts.cn

C#:   Parallel.For
来源：http://es.haigaiapp.cn

================================================================================
来源：http://jg.newstarts.cn

P. 常用工具函数
来源：http://mu.hnjuh.cn

================================================================================
来源：http://hm.hnjuh.cn

[P01] 生成 UUID
来源：http://pa.colortex.cn

Py:   str(uuid.uuid4())
来源：http://is.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qv.colortex.cn

JS:   crypto.randomUUID()
来源：http://rw.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://tj.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://jb.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://nv.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://dh.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://tw.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://sz.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jn.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nr.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://my.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://na.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ka.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jd.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jz.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pa.panjiajie.cn

[P03] 生成短随机字符串
来源：http://ac.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ic.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cg.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wq.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bp.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dw.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ad.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sq.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://go.nicolike.cn

[P04] 求长度
来源：http://cm.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vs.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://to.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zz.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ga.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://by.colortex.cn

Go:   len(arr);  len(m)
来源：http://rz.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://kw.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ot.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://xx.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ej.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cg.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vd.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ul.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uv.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ap.chemitech.net.cn

Ruby: a == b
来源：http://tg.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jo.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ki.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ji.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://sm.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wj.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://ew.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ar.colortex.cn

Go:   if x == nil {}
来源：http://kv.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fh.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://wz.yuexingan06.cn

[P07] 防抖与节流
来源：http://rr.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dj.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ud.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zu.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bx.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ba.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://db.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sy.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tq.hahajie.cn

[P08] 处理浮点精度问题
来源：http://gj.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kz.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pi.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://be.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ua.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aa.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fm.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ji.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yw.lnxyls.cn

================================================================================
来源：http://eq.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ab.bjjhwx.cn

================================================================================
来源：http://yv.9csxet.cn

[Q01] 创建表
来源：http://ob.jianghongdianzi.cn

CREATE TABLE users (
来源：http://om.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ub.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://gq.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://hn.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xv.muxihuayi.cn

);
来源：http://px.shxzukj.cn

[Q02] 创建带外键的表
来源：http://sn.szsharing.cn

CREATE TABLE orders (
来源：http://vy.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ea.shtwfgs.cn

user_id INT NOT NULL,
来源：http://bx.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://gv.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://df.szsharing.cn

);
来源：http://us.chemitech.net.cn

[Q03] 增加列
来源：http://ap.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://so.huanxung.cn

[Q04] 修改列类型
来源：http://rv.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vo.newstarts.cn

[Q05] 重命名列
来源：http://dt.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://st.shxzskj.cn

[Q06] 删除列
来源：http://ir.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://no.szxytkj.cn

[Q07] 删除表
来源：http://du.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://pv.asd995.cn

[Q08] 创建普通索引
来源：http://dv.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vu.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://vv.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qk.521024.cn

[Q10] 插入单行
来源：http://gx.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qv.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ei.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ai.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://kq.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pg.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yi.9csxet.cn

[Q13] 忽略重复插入
来源：http://hr.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zb.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://fi.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sc.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sh.szsharing.cn

[Q15] 查询全部
来源：http://es.muxihuayi.cn

SELECT * FROM users;
来源：http://ra.hnjuh.cn

[Q16] 查询指定列
来源：http://wz.521024.cn

SELECT id, name FROM users;
来源：http://qy.szsharing.cn

[Q17] 条件查询
来源：http://qx.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yq.lnxyls.cn

[Q18] 模糊匹配
来源：http://cn.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nm.yuexingan06.cn

[Q19] 范围查询
来源：http://gz.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ib.szxytkj.cn

[Q20] IN 列表
来源：http://qd.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dk.szxytkj.cn

[Q21] 空值判断
来源：http://ot.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xk.shxzskj.cn

[Q22] 排序
来源：http://mp.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cb.huixinmuqiang.cn

[Q23] 分页
来源：http://nm.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ah.lnxyls.cn

[Q24] 去重
来源：http://sz.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://jh.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://ob.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fr.shtwfgs.cn

[Q26] 计数
来源：http://on.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://hs.bjjhwx.cn

[Q27] 条件计数
来源：http://db.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zy.panjiajie.cn

[Q28] 求和与平均
来源：http://xy.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://op.521024.cn

[Q29] 最大最小值
来源：http://ro.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nn.gzmigu.cn

[Q30] 分组统计
来源：http://kb.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xh.wgjwhj.cn

[Q31] 分组后过滤
来源：http://xy.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hx.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://bi.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qv.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nz.shxzukj.cn

[Q33] 多列分组
来源：http://qk.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iz.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://vs.521024.cn

SELECT * FROM (
来源：http://qo.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://om.asd995.cn

) t WHERE rn = 1;
来源：http://ol.panjiajie.cn

[Q35] 内连接
来源：http://mp.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aj.nszjky.cn

[Q36] 左连接
来源：http://rx.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zn.huixiangedu.cn

[Q37] 右连接
来源：http://in.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tq.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qb.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vu.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://sk.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://et.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lx.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lo.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://td.521024.cn

[Q41] 多表连接
来源：http://gr.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ma.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://go.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://gy.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://mi.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://tr.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://za.haigaiapp.cn

[Q43] 标量子查询
来源：http://tl.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cf.hahajie.cn

[Q44] IN 子查询
来源：http://zr.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hj.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ef.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dx.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xv.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tp.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ey.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mf.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://mo.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yj.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://qt.shxzskj.cn

[Q49] 更新单行
来源：http://zm.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vi.lnxyls.cn

[Q50] 批量更新
来源：http://js.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hi.gzmigu.cn

[Q51] 用子查询更新
来源：http://xp.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vy.colortex.cn

[Q52] 删除指定行
来源：http://ug.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://xz.shtwfgs.cn

[Q53] 按条件删除
来源：http://ka.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uu.nicolike.cn

[Q54] 清空表
来源：http://qb.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://mt.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://du.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yc.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://cy.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pw.colortex.cn

[Q57] 行号
来源：http://zv.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sm.wgjwhj.cn

[Q58] 累计求和
来源：http://wf.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mc.newstarts.cn

[Q59] 分组内累计
来源：http://pv.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mh.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://bu.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rj.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mm.colortex.cn

[Q61] 移动平均
来源：http://qc.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vt.huanxung.cn

[Q62] 分组占比
来源：http://wp.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lx.jianghongdianzi.cn

[Q63] 开启事务
来源：http://fk.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sy.newstarts.cn

[Q64] 提交事务
来源：http://rp.muxihuayi.cn

COMMIT;
来源：http://hu.jctech888.com.cn

[Q65] 回滚事务
来源：http://dv.szxytkj.cn

ROLLBACK;
来源：http://zc.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://xl.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mj.shxzskj.cn

[Q67] 设置隔离级别
来源：http://cz.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fc.nszjky.cn

[Q68] 保存点
来源：http://mw.huanxung.cn

SAVEPOINT sp1;
来源：http://qn.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://vl.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://mh.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kr.newstarts.cn

[Q70] 更新统计信息
来源：http://ui.szxytkj.cn

ANALYZE TABLE users;
来源：http://ie.huixiangedu.cn

[Q71] 查看建表语句
来源：http://xi.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zh.muxihuayi.cn

[Q72] 查看索引
来源：http://zm.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://ox.shxzukj.cn

[Q73] 查看表状态
来源：http://ov.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wa.szsharing.cn

[Q74] 强制使用索引
来源：http://ck.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xf.haigaiapp.cn

[Q75] 日期格式化
来源：http://cy.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cd.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kf.bookmarksfly.cn


<!-- 参考信息 -->