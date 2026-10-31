代发 wailian999

[O02] 使用线程池
来源：http://qe.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fh.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bg.newstarts.cn

JS:   // worker_threads 线程池
来源：http://my.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://tu.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ss.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fo.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://go.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://md.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://al.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://ef.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://un.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ze.yuexingan06.cn

TS:   // 同 JS
来源：http://kq.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://cn.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cu.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xe.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://db.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://nk.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://fa.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pd.szsharing.cn

JS:   async function f() { await g(); }
来源：http://xc.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://om.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kt.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ee.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wd.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://eg.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://cf.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://lk.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ir.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ue.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://nj.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://su.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pr.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://vt.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bi.huanxung.cn

[O06] 使用进程池
来源：http://up.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ac.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ol.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://ad.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://ix.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://or.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://of.muxihuayi.cn

Ruby: // fork 块
来源：http://qk.huixiangedu.cn

C#:   Parallel.For
来源：http://aa.bjjhwx.cn

================================================================================
来源：http://pw.yuntaijiaju.cn

P. 常用工具函数
来源：http://rs.wgjwhj.cn

================================================================================
来源：http://mk.hnjuh.cn

[P01] 生成 UUID
来源：http://tm.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://ue.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zx.nicolike.cn

JS:   crypto.randomUUID()
来源：http://wd.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://xt.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://vn.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://uh.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://xj.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://mk.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://vw.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://em.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eq.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ig.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dl.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zz.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cc.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dq.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qy.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://rc.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hf.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lc.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aj.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rx.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lq.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xy.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rg.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ho.asd995.cn

[P04] 求长度
来源：http://lm.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://it.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rh.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qa.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mv.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://fm.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://iu.szxytkj.cn

Ruby: x.length;  x.size
来源：http://tj.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jv.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://su.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sn.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vg.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lx.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mv.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aa.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zd.521024.cn

Ruby: a == b
来源：http://sx.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qa.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ej.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sc.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://aa.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fg.bjjhwx.cn

TS:   if (x == null) {}
来源：http://ly.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dm.lnxyls.cn

Go:   if x == nil {}
来源：http://qd.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qq.colortex.cn

C#:   if (x is null) {}
来源：http://ap.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://eq.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ho.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://jl.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yd.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mn.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sj.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yc.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mg.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lm.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://il.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kb.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bq.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ed.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qp.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zo.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ov.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fe.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xp.szxytkj.cn

================================================================================
来源：http://ph.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://da.jctech888.com.cn

================================================================================
来源：http://rv.shtwfgs.cn

[Q01] 创建表
来源：http://jm.jianghongdianzi.cn

CREATE TABLE users (
来源：http://tx.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zg.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://nz.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://nd.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gx.nszjky.cn

);
来源：http://nw.newstarts.cn

[Q02] 创建带外键的表
来源：http://oq.panjiajie.cn

CREATE TABLE orders (
来源：http://os.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dy.szsharing.cn

user_id INT NOT NULL,
来源：http://tq.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://xj.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wc.haigaiapp.cn

);
来源：http://qg.asd995.cn

[Q03] 增加列
来源：http://xi.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mm.colortex.cn

[Q04] 修改列类型
来源：http://jn.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fv.bjjhwx.cn

[Q05] 重命名列
来源：http://ui.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nl.bookmarksfly.cn

[Q06] 删除列
来源：http://ni.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lq.yuexingan06.cn

[Q07] 删除表
来源：http://dl.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://uc.szsharing.cn

[Q08] 创建普通索引
来源：http://bq.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dw.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://dr.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hr.nicolike.cn

[Q10] 插入单行
来源：http://eq.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kq.shxzskj.cn

[Q11] 一次插入多行
来源：http://le.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ih.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://ii.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mf.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tc.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://ov.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lr.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://qp.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fo.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kv.haigaiapp.cn

[Q15] 查询全部
来源：http://oe.hnjuh.cn

SELECT * FROM users;
来源：http://tm.haigaiapp.cn

[Q16] 查询指定列
来源：http://sm.yuexingan06.cn

SELECT id, name FROM users;
来源：http://np.hahajie.cn

[Q17] 条件查询
来源：http://xq.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://du.yuexingan06.cn

[Q18] 模糊匹配
来源：http://pm.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lf.newstarts.cn

[Q19] 范围查询
来源：http://zw.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ei.asd995.cn

[Q20] IN 列表
来源：http://vc.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bw.jctech888.com.cn

[Q21] 空值判断
来源：http://mr.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kl.newstarts.cn

[Q22] 排序
来源：http://wq.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cl.nicolike.cn

[Q23] 分页
来源：http://oe.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jc.panjiajie.cn

[Q24] 去重
来源：http://sx.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://fz.shxzskj.cn

[Q25] 只取前 N 条
来源：http://tf.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zd.shtwfgs.cn

[Q26] 计数
来源：http://fo.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://de.chemitech.net.cn

[Q27] 条件计数
来源：http://br.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shxzskj.cn

[Q28] 求和与平均
来源：http://tr.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jl.gzmigu.cn

[Q29] 最大最小值
来源：http://pm.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mw.9csxet.cn

[Q30] 分组统计
来源：http://qh.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xl.szsharing.cn

[Q31] 分组后过滤
来源：http://gn.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ip.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://av.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nr.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yj.szxytkj.cn

[Q33] 多列分组
来源：http://ra.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zy.szsharing.cn

[Q34] 每组取第一条
来源：http://go.shxzskj.cn

SELECT * FROM (
来源：http://yi.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ph.chemitech.net.cn

) t WHERE rn = 1;
来源：http://qb.muxihuayi.cn

[Q35] 内连接
来源：http://fu.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ae.huanxung.cn

[Q36] 左连接
来源：http://ph.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lv.yuexingan06.cn

[Q37] 右连接
来源：http://ih.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://en.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ok.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cl.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://ds.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gq.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ag.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jc.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pm.shtwfgs.cn

[Q41] 多表连接
来源：http://px.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yg.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://rz.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://ni.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://zl.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://hy.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eu.shtwfgs.cn

[Q43] 标量子查询
来源：http://ui.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kl.asd995.cn

[Q44] IN 子查询
来源：http://yo.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vu.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://jt.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nk.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bt.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ws.muxihuayi.cn

[Q47] 与平均值比较
来源：http://wf.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ou.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://al.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tf.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://gs.shtwfgs.cn

[Q49] 更新单行
来源：http://uk.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ve.jianghongdianzi.cn

[Q50] 批量更新
来源：http://yz.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://np.9csxet.cn

[Q51] 用子查询更新
来源：http://xj.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dx.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://hv.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://fb.bookmarksfly.cn

[Q53] 按条件删除
来源：http://pj.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ta.lnxyls.cn

[Q54] 清空表
来源：http://bn.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://fw.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://rn.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://os.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://gm.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zq.hnjuh.cn

[Q57] 行号
来源：http://nn.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hb.jctech888.com.cn

[Q58] 累计求和
来源：http://id.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ua.lnxyls.cn

[Q59] 分组内累计
来源：http://sy.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aj.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://da.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bx.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vn.yuexingan06.cn

[Q61] 移动平均
来源：http://ya.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tj.asd995.cn

[Q62] 分组占比
来源：http://nf.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qv.newstarts.cn

[Q63] 开启事务
来源：http://xs.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cw.chemitech.net.cn

[Q64] 提交事务
来源：http://vp.hnjuh.cn

COMMIT;
来源：http://go.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://ay.wgjwhj.cn

ROLLBACK;
来源：http://pu.bjjhwx.cn

[Q66] 行锁查询
来源：http://qv.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xo.shxzskj.cn

[Q67] 设置隔离级别
来源：http://vd.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vo.shxzukj.cn

[Q68] 保存点
来源：http://bj.jctech888.com.cn

SAVEPOINT sp1;
来源：http://de.9csxet.cn

ROLLBACK TO sp1;
来源：http://gv.huixiangedu.cn

[Q69] 查看执行计划
来源：http://sy.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nt.nszjky.cn

[Q70] 更新统计信息
来源：http://cq.yuexingan06.cn

ANALYZE TABLE users;
来源：http://mh.jctech888.com.cn

[Q71] 查看建表语句
来源：http://rz.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yh.asd995.cn

[Q72] 查看索引
来源：http://ml.521024.cn

SHOW INDEX FROM users;
来源：http://gb.shtwfgs.cn

[Q73] 查看表状态
来源：http://iy.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uw.521024.cn

[Q74] 强制使用索引
来源：http://ug.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vd.haigaiapp.cn

[Q75] 日期格式化
来源：http://ln.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iy.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rp.haigaiapp.cn

[Q76] 按天统计
来源：http://hw.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vj.jianghongdianzi.cn

[Q77] 时间加减
来源：http://en.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ex.gzmigu.cn


<!-- 参考信息 -->