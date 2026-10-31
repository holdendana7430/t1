代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://dm.jianghongdianzi.cn

Go:   go f()
来源：http://wp.521024.cn

Ruby: Thread.new { f }
来源：http://gn.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://zw.huixiangedu.cn

[O02] 使用线程池
来源：http://eb.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hu.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yd.9csxet.cn

JS:   // worker_threads 线程池
来源：http://fm.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://vd.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lu.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nn.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mb.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tb.9csxet.cn

[O03] 加锁保护共享数据
来源：http://ht.nszjky.cn

Py:   with lock: shared += 1
来源：http://fl.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ru.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xt.jctech888.com.cn

TS:   // 同 JS
来源：http://qk.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://qf.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dj.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gf.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://nf.nszjky.cn

[O04] 定义异步函数并等待
来源：http://am.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://yo.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tr.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://tq.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://df.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qh.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ez.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tz.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://wv.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://xg.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://qf.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ya.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://zz.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://zg.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nf.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ml.colortex.cn

Ruby: threads.map(&:join)
来源：http://bd.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vr.haigaiapp.cn

[O06] 使用进程池
来源：http://jq.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qr.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zm.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://ja.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://pu.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ln.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gs.colortex.cn

Ruby: // fork 块
来源：http://yq.szxytkj.cn

C#:   Parallel.For
来源：http://jt.shxzukj.cn

================================================================================
来源：http://do.gzmigu.cn

P. 常用工具函数
来源：http://nr.nszjky.cn

================================================================================
来源：http://bx.panjiajie.cn

[P01] 生成 UUID
来源：http://ls.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://ei.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://il.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://gs.colortex.cn

TS:   crypto.randomUUID()
来源：http://je.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://fo.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ec.521024.cn

Ruby: SecureRandom.uuid
来源：http://de.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://ta.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://yy.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cm.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wv.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ti.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eh.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uh.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zm.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pt.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mr.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://kr.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sw.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ft.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ca.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://va.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fs.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rl.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ao.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lr.nicolike.cn

[P04] 求长度
来源：http://kr.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qe.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eh.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xv.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ss.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://in.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://vs.asd995.cn

Ruby: x.length;  x.size
来源：http://io.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hb.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://gp.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wx.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xc.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ha.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yn.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pe.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wq.newstarts.cn

Ruby: a == b
来源：http://ld.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tn.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bp.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wr.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://db.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vj.szsharing.cn

TS:   if (x == null) {}
来源：http://ln.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bd.huanxung.cn

Go:   if x == nil {}
来源：http://wy.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ms.chemitech.net.cn

C#:   if (x is null) {}
来源：http://dv.colortex.cn

[P07] 防抖与节流
来源：http://jd.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yr.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://yp.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://km.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fv.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://le.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ry.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qn.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aq.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://yo.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pp.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pm.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zp.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ok.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xb.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dg.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ir.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://td.yuntaijiaju.cn

================================================================================
来源：http://au.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zu.gzmigu.cn

================================================================================
来源：http://oa.jianghongdianzi.cn

[Q01] 创建表
来源：http://qx.9csxet.cn

CREATE TABLE users (
来源：http://lp.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dh.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://xt.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://mz.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qe.gzmigu.cn

);
来源：http://tw.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://rd.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://nj.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oe.huixiangedu.cn

user_id INT NOT NULL,
来源：http://cu.huanxung.cn

amount DECIMAL(10, 2),
来源：http://qn.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cy.bjjhwx.cn

);
来源：http://bn.bookmarksfly.cn

[Q03] 增加列
来源：http://sl.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://di.panjiajie.cn

[Q04] 修改列类型
来源：http://cd.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qd.gzmigu.cn

[Q05] 重命名列
来源：http://hq.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fu.521024.cn

[Q06] 删除列
来源：http://og.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yy.bjjhwx.cn

[Q07] 删除表
来源：http://nr.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://yg.jctech888.com.cn

[Q08] 创建普通索引
来源：http://cc.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sj.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://pd.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uv.newstarts.cn

[Q10] 插入单行
来源：http://vd.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ug.hahajie.cn

[Q11] 一次插入多行
来源：http://kf.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rp.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://yq.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xu.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ab.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://lr.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ob.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://lr.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nt.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jl.muxihuayi.cn

[Q15] 查询全部
来源：http://mi.shxzskj.cn

SELECT * FROM users;
来源：http://mn.jctech888.com.cn

[Q16] 查询指定列
来源：http://tw.asd995.cn

SELECT id, name FROM users;
来源：http://sh.bookmarksfly.cn

[Q17] 条件查询
来源：http://mx.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hw.yuexingan06.cn

[Q18] 模糊匹配
来源：http://ey.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hq.bookmarksfly.cn

[Q19] 范围查询
来源：http://hw.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zs.bookmarksfly.cn

[Q20] IN 列表
来源：http://ju.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nz.bjjhwx.cn

[Q21] 空值判断
来源：http://ss.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qi.wgjwhj.cn

[Q22] 排序
来源：http://yr.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ny.newstarts.cn

[Q23] 分页
来源：http://ml.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hn.9csxet.cn

[Q24] 去重
来源：http://jz.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://ld.panjiajie.cn

[Q25] 只取前 N 条
来源：http://eo.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://el.colortex.cn

[Q26] 计数
来源：http://fe.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://ot.lnxyls.cn

[Q27] 条件计数
来源：http://id.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qw.szsharing.cn

[Q28] 求和与平均
来源：http://hb.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ze.newstarts.cn

[Q29] 最大最小值
来源：http://ku.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jh.yuexingan06.cn

[Q30] 分组统计
来源：http://ey.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pm.shxzukj.cn

[Q31] 分组后过滤
来源：http://bn.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xl.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://vk.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ri.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ra.bookmarksfly.cn

[Q33] 多列分组
来源：http://xf.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://op.szsharing.cn

[Q34] 每组取第一条
来源：http://pl.wgjwhj.cn

SELECT * FROM (
来源：http://oy.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oo.jctech888.com.cn

) t WHERE rn = 1;
来源：http://qy.gzmigu.cn

[Q35] 内连接
来源：http://vl.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ly.521024.cn

[Q36] 左连接
来源：http://fg.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://py.9csxet.cn

[Q37] 右连接
来源：http://ic.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sq.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ux.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gw.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://ma.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wr.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wk.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ce.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lm.hnjuh.cn

[Q41] 多表连接
来源：http://yw.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://br.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://pv.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ur.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://fs.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://nn.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nz.9csxet.cn

[Q43] 标量子查询
来源：http://kv.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rl.yuexingan06.cn

[Q44] IN 子查询
来源：http://gq.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rt.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://sl.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jx.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ok.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vu.colortex.cn

[Q47] 与平均值比较
来源：http://oq.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ei.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://qs.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ev.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://de.jianghongdianzi.cn

[Q49] 更新单行
来源：http://bk.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lj.yuntaijiaju.cn

[Q50] 批量更新
来源：http://aa.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ua.szsharing.cn

[Q51] 用子查询更新
来源：http://bo.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bd.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://br.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://nz.muxihuayi.cn

[Q53] 按条件删除
来源：http://mz.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://az.521024.cn

[Q54] 清空表
来源：http://ts.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://sy.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://kb.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gk.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://dt.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sx.colortex.cn

[Q57] 行号
来源：http://ex.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lc.haigaiapp.cn

[Q58] 累计求和
来源：http://mg.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lb.lnxyls.cn

[Q59] 分组内累计
来源：http://ba.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ip.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://wa.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qo.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kw.jctech888.com.cn

[Q61] 移动平均
来源：http://gy.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ni.colortex.cn

[Q62] 分组占比
来源：http://qo.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cy.lnxyls.cn

[Q63] 开启事务
来源：http://zx.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mp.chemitech.net.cn

[Q64] 提交事务
来源：http://pc.yuntaijiaju.cn

COMMIT;
来源：http://na.asd995.cn

[Q65] 回滚事务
来源：http://ut.nicolike.cn

ROLLBACK;
来源：http://ii.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://po.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yq.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://hk.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kd.gzmigu.cn

[Q68] 保存点
来源：http://ol.hahajie.cn

SAVEPOINT sp1;
来源：http://og.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://wy.bjjhwx.cn

[Q69] 查看执行计划
来源：http://vv.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iv.huanxung.cn

[Q70] 更新统计信息
来源：http://oe.bjjhwx.cn

ANALYZE TABLE users;
来源：http://bg.nszjky.cn

[Q71] 查看建表语句
来源：http://ms.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nc.shtwfgs.cn

[Q72] 查看索引
来源：http://uw.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://aa.hahajie.cn

[Q73] 查看表状态
来源：http://ih.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gt.gzmigu.cn

[Q74] 强制使用索引
来源：http://rf.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ls.shtwfgs.cn

[Q75] 日期格式化
来源：http://jr.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tg.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://no.haigaiapp.cn


<!-- 参考信息 -->