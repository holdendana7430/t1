代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://ao.haigaiapp.cn

Go:   go f()
来源：http://hx.nicolike.cn

Ruby: Thread.new { f }
来源：http://hj.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://lx.colortex.cn

[O02] 使用线程池
来源：http://yr.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ho.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ta.szsharing.cn

JS:   // worker_threads 线程池
来源：http://iq.asd995.cn

TS:   // worker_threads 线程池
来源：http://by.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mb.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bv.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oq.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://or.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://cf.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://iw.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ju.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ii.wgjwhj.cn

TS:   // 同 JS
来源：http://ws.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://vs.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kd.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://je.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://vn.hahajie.cn

[O04] 定义异步函数并等待
来源：http://yr.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://hk.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xr.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://mv.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://op.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kz.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qh.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gg.colortex.cn

C#:   async Task F() { await G(); }
来源：http://qx.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://yj.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://wc.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tx.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://yd.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://yx.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ct.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wa.hahajie.cn

Ruby: threads.map(&:join)
来源：http://wn.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://et.colortex.cn

[O06] 使用进程池
来源：http://ci.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mi.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gf.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://jp.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://pk.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oy.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hb.jctech888.com.cn

Ruby: // fork 块
来源：http://to.newstarts.cn

C#:   Parallel.For
来源：http://ds.9csxet.cn

================================================================================
来源：http://nd.newstarts.cn

P. 常用工具函数
来源：http://zm.chemitech.net.cn

================================================================================
来源：http://sb.asd995.cn

[P01] 生成 UUID
来源：http://yn.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://lx.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ul.newstarts.cn

JS:   crypto.randomUUID()
来源：http://xu.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://qi.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://nm.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://bw.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://yi.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://pn.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://wr.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ij.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qi.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dc.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://si.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mx.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pt.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kv.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fh.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://rb.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yj.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qw.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xf.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fm.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gb.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ea.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bh.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ag.jianghongdianzi.cn

[P04] 求长度
来源：http://zl.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://on.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xm.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://of.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ju.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://gj.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://ei.szsharing.cn

Ruby: x.length;  x.size
来源：http://rv.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xp.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://pf.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://al.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://va.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ng.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://go.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gv.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zf.huixinmuqiang.cn

Ruby: a == b
来源：http://ka.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nl.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pz.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wy.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://vg.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ux.haigaiapp.cn

TS:   if (x == null) {}
来源：http://oj.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gt.wgjwhj.cn

Go:   if x == nil {}
来源：http://jq.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ck.hahajie.cn

C#:   if (x is null) {}
来源：http://nv.shxzukj.cn

[P07] 防抖与节流
来源：http://lx.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hl.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ma.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ef.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jn.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://df.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kr.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jp.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pk.nszjky.cn

[P08] 处理浮点精度问题
来源：http://mf.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gh.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qj.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nc.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://od.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ff.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ns.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ff.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://of.colortex.cn

================================================================================
来源：http://qc.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qx.newstarts.cn

================================================================================
来源：http://ar.lnxyls.cn

[Q01] 创建表
来源：http://ga.colortex.cn

CREATE TABLE users (
来源：http://eg.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cd.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://bl.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://ak.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hp.hnjuh.cn

);
来源：http://uj.lnxyls.cn

[Q02] 创建带外键的表
来源：http://rs.haigaiapp.cn

CREATE TABLE orders (
来源：http://ki.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dv.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://vs.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://zj.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jy.yuexingan06.cn

);
来源：http://xe.huixiangedu.cn

[Q03] 增加列
来源：http://lm.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jw.huanxung.cn

[Q04] 修改列类型
来源：http://cb.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rt.chemitech.net.cn

[Q05] 重命名列
来源：http://wu.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ju.shxzukj.cn

[Q06] 删除列
来源：http://ur.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ht.yuexingan06.cn

[Q07] 删除表
来源：http://ve.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://xt.hnjuh.cn

[Q08] 创建普通索引
来源：http://ef.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rs.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://hk.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uz.chemitech.net.cn

[Q10] 插入单行
来源：http://zt.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pj.bjjhwx.cn

[Q11] 一次插入多行
来源：http://ra.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dz.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://td.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iw.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fk.nicolike.cn

[Q13] 忽略重复插入
来源：http://bs.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eb.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://ok.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gb.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tk.szxytkj.cn

[Q15] 查询全部
来源：http://yz.muxihuayi.cn

SELECT * FROM users;
来源：http://fn.chemitech.net.cn

[Q16] 查询指定列
来源：http://uy.shxzukj.cn

SELECT id, name FROM users;
来源：http://wb.newstarts.cn

[Q17] 条件查询
来源：http://jr.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pb.asd995.cn

[Q18] 模糊匹配
来源：http://ub.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wl.shtwfgs.cn

[Q19] 范围查询
来源：http://xq.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tt.lnxyls.cn

[Q20] IN 列表
来源：http://eg.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wj.shxzukj.cn

[Q21] 空值判断
来源：http://aq.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tb.bookmarksfly.cn

[Q22] 排序
来源：http://dv.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jl.hahajie.cn

[Q23] 分页
来源：http://ei.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oj.asd995.cn

[Q24] 去重
来源：http://nq.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://hw.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://dj.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xc.gzmigu.cn

[Q26] 计数
来源：http://el.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://bu.chemitech.net.cn

[Q27] 条件计数
来源：http://gh.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kt.huanxung.cn

[Q28] 求和与平均
来源：http://qb.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ln.shxzukj.cn

[Q29] 最大最小值
来源：http://do.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tl.panjiajie.cn

[Q30] 分组统计
来源：http://fg.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fy.panjiajie.cn

[Q31] 分组后过滤
来源：http://rm.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bq.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://te.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xd.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lh.huanxung.cn

[Q33] 多列分组
来源：http://eq.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bs.panjiajie.cn

[Q34] 每组取第一条
来源：http://ol.chemitech.net.cn

SELECT * FROM (
来源：http://tv.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eq.huixiangedu.cn

) t WHERE rn = 1;
来源：http://li.panjiajie.cn

[Q35] 内连接
来源：http://mp.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ib.yuntaijiaju.cn

[Q36] 左连接
来源：http://gi.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rg.yuexingan06.cn

[Q37] 右连接
来源：http://pf.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://df.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sa.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://co.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://ds.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://md.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mu.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jl.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kp.muxihuayi.cn

[Q41] 多表连接
来源：http://rc.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rn.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://zp.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://oa.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://sh.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://np.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://me.nicolike.cn

[Q43] 标量子查询
来源：http://uv.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qt.huixiangedu.cn

[Q44] IN 子查询
来源：http://ed.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://im.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://il.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pk.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zc.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xe.gzmigu.cn

[Q47] 与平均值比较
来源：http://bw.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yy.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://qa.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lx.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://jg.wgjwhj.cn

[Q49] 更新单行
来源：http://tq.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eb.9csxet.cn

[Q50] 批量更新
来源：http://xo.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://my.huanxung.cn

[Q51] 用子查询更新
来源：http://ru.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://su.muxihuayi.cn

[Q52] 删除指定行
来源：http://jo.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://oi.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://wq.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nc.chemitech.net.cn

[Q54] 清空表
来源：http://uz.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ue.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ya.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ua.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://rk.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ls.szsharing.cn

[Q57] 行号
来源：http://su.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dy.huanxung.cn

[Q58] 累计求和
来源：http://od.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vg.yuexingan06.cn

[Q59] 分组内累计
来源：http://ua.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nt.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://xt.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pq.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wu.shtwfgs.cn

[Q61] 移动平均
来源：http://bo.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ms.gzmigu.cn

[Q62] 分组占比
来源：http://ng.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ts.newstarts.cn

[Q63] 开启事务
来源：http://vh.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ur.shtwfgs.cn

[Q64] 提交事务
来源：http://kg.bjjhwx.cn

COMMIT;
来源：http://eg.muxihuayi.cn

[Q65] 回滚事务
来源：http://iy.szsharing.cn

ROLLBACK;
来源：http://qf.panjiajie.cn

[Q66] 行锁查询
来源：http://xg.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://md.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://xl.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hm.panjiajie.cn

[Q68] 保存点
来源：http://jx.521024.cn

SAVEPOINT sp1;
来源：http://fm.nicolike.cn

ROLLBACK TO sp1;
来源：http://aa.szsharing.cn

[Q69] 查看执行计划
来源：http://ig.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wp.muxihuayi.cn

[Q70] 更新统计信息
来源：http://pd.nicolike.cn

ANALYZE TABLE users;
来源：http://zz.newstarts.cn

[Q71] 查看建表语句
来源：http://vp.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oz.newstarts.cn

[Q72] 查看索引
来源：http://mb.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://ce.hnjuh.cn

[Q73] 查看表状态
来源：http://zx.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bv.newstarts.cn

[Q74] 强制使用索引
来源：http://we.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ln.asd995.cn

[Q75] 日期格式化
来源：http://mp.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yi.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jk.szsharing.cn


<!-- 参考信息 -->