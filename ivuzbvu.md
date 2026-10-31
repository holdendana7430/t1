代发 wailian999

TS:   // worker_threads 线程池
来源：http://nf.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ol.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cu.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qh.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oj.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://vb.szsharing.cn

Py:   with lock: shared += 1
来源：http://ph.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://jt.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nd.wgjwhj.cn

TS:   // 同 JS
来源：http://zt.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://zk.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bn.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kl.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://mi.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://as.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://kw.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cw.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://ks.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nn.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://od.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aj.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://on.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://nk.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://we.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://ii.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yb.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://vg.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://ta.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wa.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zk.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://bn.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mr.hnjuh.cn

[O06] 使用进程池
来源：http://ry.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fj.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ha.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://lh.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://lp.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uo.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cz.muxihuayi.cn

Ruby: // fork 块
来源：http://bh.newstarts.cn

C#:   Parallel.For
来源：http://km.nszjky.cn

================================================================================
来源：http://ro.haigaiapp.cn

P. 常用工具函数
来源：http://pa.nszjky.cn

================================================================================
来源：http://aw.bookmarksfly.cn

[P01] 生成 UUID
来源：http://zn.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://rb.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tr.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://zg.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://ai.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://le.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://rj.colortex.cn

Ruby: SecureRandom.uuid
来源：http://bi.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://pf.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://bx.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lb.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fd.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iy.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ma.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hr.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hw.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yr.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dl.szsharing.cn

[P03] 生成短随机字符串
来源：http://zh.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gx.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nd.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qi.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pg.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cv.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sk.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mi.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iy.chemitech.net.cn

[P04] 求长度
来源：http://rn.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mf.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rj.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fi.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://do.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://mt.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://oo.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pv.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://oi.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zz.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xu.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zp.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ia.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mm.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ce.bjjhwx.cn

Ruby: a == b
来源：http://mq.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cu.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fi.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ir.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://gg.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ra.muxihuayi.cn

TS:   if (x == null) {}
来源：http://yj.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fe.521024.cn

Go:   if x == nil {}
来源：http://kv.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ha.huixiangedu.cn

C#:   if (x is null) {}
来源：http://dn.chemitech.net.cn

[P07] 防抖与节流
来源：http://rj.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rp.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://cr.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tk.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fb.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ih.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zd.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hd.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ee.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://uq.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bg.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ax.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://un.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lg.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ih.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xi.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://do.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bb.chemitech.net.cn

================================================================================
来源：http://px.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nf.szxytkj.cn

================================================================================
来源：http://xl.huanxung.cn

[Q01] 创建表
来源：http://ek.9csxet.cn

CREATE TABLE users (
来源：http://es.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wb.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://sn.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://rf.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gn.colortex.cn

);
来源：http://ab.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://yl.bjjhwx.cn

CREATE TABLE orders (
来源：http://yd.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oy.szsharing.cn

user_id INT NOT NULL,
来源：http://ol.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://mb.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eg.muxihuayi.cn

);
来源：http://au.shxzskj.cn

[Q03] 增加列
来源：http://ku.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nj.szsharing.cn

[Q04] 修改列类型
来源：http://oe.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fp.szxytkj.cn

[Q05] 重命名列
来源：http://vk.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mc.colortex.cn

[Q06] 删除列
来源：http://gi.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rq.chemitech.net.cn

[Q07] 删除表
来源：http://nk.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://av.shxzskj.cn

[Q08] 创建普通索引
来源：http://pn.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ew.521024.cn

[Q09] 创建唯一索引
来源：http://cd.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bx.asd995.cn

[Q10] 插入单行
来源：http://vq.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rf.shxzukj.cn

[Q11] 一次插入多行
来源：http://ll.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nj.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://io.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pb.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rj.shxzukj.cn

[Q13] 忽略重复插入
来源：http://xx.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sp.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://bn.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dl.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ln.wgjwhj.cn

[Q15] 查询全部
来源：http://ym.szsharing.cn

SELECT * FROM users;
来源：http://ax.huixiangedu.cn

[Q16] 查询指定列
来源：http://it.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://ql.huanxung.cn

[Q17] 条件查询
来源：http://sr.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ug.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://ld.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ok.wgjwhj.cn

[Q19] 范围查询
来源：http://fj.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://re.yuexingan06.cn

[Q20] IN 列表
来源：http://aj.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tj.asd995.cn

[Q21] 空值判断
来源：http://zx.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cz.haigaiapp.cn

[Q22] 排序
来源：http://gi.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bv.yuexingan06.cn

[Q23] 分页
来源：http://qr.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rv.bookmarksfly.cn

[Q24] 去重
来源：http://zu.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://wc.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://iw.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lx.521024.cn

[Q26] 计数
来源：http://px.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://wq.shxzskj.cn

[Q27] 条件计数
来源：http://fp.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ph.shxzukj.cn

[Q28] 求和与平均
来源：http://uw.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qr.lnxyls.cn

[Q29] 最大最小值
来源：http://jz.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ik.521024.cn

[Q30] 分组统计
来源：http://tg.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rj.haigaiapp.cn

[Q31] 分组后过滤
来源：http://jc.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qf.szsharing.cn

[Q32] 分组拼接字符串
来源：http://yx.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vc.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jk.nicolike.cn

[Q33] 多列分组
来源：http://jm.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oo.nicolike.cn

[Q34] 每组取第一条
来源：http://wu.nszjky.cn

SELECT * FROM (
来源：http://aq.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jc.szsharing.cn

) t WHERE rn = 1;
来源：http://wz.muxihuayi.cn

[Q35] 内连接
来源：http://cl.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wk.asd995.cn

[Q36] 左连接
来源：http://mu.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qv.chemitech.net.cn

[Q37] 右连接
来源：http://eq.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fu.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kl.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vq.colortex.cn

[Q39] 自连接（查上下级）
来源：http://ie.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gt.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kq.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nr.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gc.haigaiapp.cn

[Q41] 多表连接
来源：http://sp.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vp.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://et.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://kf.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://os.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://xq.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wb.wgjwhj.cn

[Q43] 标量子查询
来源：http://gu.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ep.shtwfgs.cn

[Q44] IN 子查询
来源：http://wt.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ee.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ud.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sg.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eb.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hd.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://ph.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://im.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://uj.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qv.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://yj.hnjuh.cn

[Q49] 更新单行
来源：http://zf.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://me.wgjwhj.cn

[Q50] 批量更新
来源：http://bz.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zs.bjjhwx.cn

[Q51] 用子查询更新
来源：http://xl.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ao.huixiangedu.cn

[Q52] 删除指定行
来源：http://yt.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://cs.shtwfgs.cn

[Q53] 按条件删除
来源：http://fd.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ni.hnjuh.cn

[Q54] 清空表
来源：http://fl.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://hm.newstarts.cn

[Q55] 排名（并列占位）
来源：http://ng.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gm.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://ly.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zj.nszjky.cn

[Q57] 行号
来源：http://bh.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qb.shtwfgs.cn

[Q58] 累计求和
来源：http://ew.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kn.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://bw.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vq.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://ra.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cx.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oo.panjiajie.cn

[Q61] 移动平均
来源：http://lf.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sk.hahajie.cn

[Q62] 分组占比
来源：http://kp.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rw.hnjuh.cn

[Q63] 开启事务
来源：http://hm.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ar.szsharing.cn

[Q64] 提交事务
来源：http://cx.hahajie.cn

COMMIT;
来源：http://ek.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://rj.asd995.cn

ROLLBACK;
来源：http://rz.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://ur.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vr.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://xe.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rk.nszjky.cn

[Q68] 保存点
来源：http://aj.shxzskj.cn

SAVEPOINT sp1;
来源：http://an.shxzukj.cn

ROLLBACK TO sp1;
来源：http://zc.shxzukj.cn

[Q69] 查看执行计划
来源：http://br.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ks.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://fz.huixiangedu.cn

ANALYZE TABLE users;
来源：http://up.shxzskj.cn

[Q71] 查看建表语句
来源：http://cj.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cm.gzmigu.cn

[Q72] 查看索引
来源：http://sl.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://fu.chemitech.net.cn

[Q73] 查看表状态
来源：http://dm.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tc.gzmigu.cn

[Q74] 强制使用索引
来源：http://pv.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vl.huanxung.cn

[Q75] 日期格式化
来源：http://qz.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ry.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iv.yuexingan06.cn

[Q76] 按天统计
来源：http://cq.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ij.yuexingan06.cn

[Q77] 时间加减
来源：http://ch.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yl.jianghongdianzi.cn

[Q78] 当前时间
来源：http://xi.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lv.shxzukj.cn

[Q79] 字符串拼接
来源：http://jh.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pm.hnjuh.cn


<!-- 参考信息 -->