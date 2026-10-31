代发 wailian999

[O02] 使用线程池
来源：http://sr.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ty.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vp.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://nz.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://zs.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hq.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dv.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sg.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jf.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://rt.nszjky.cn

Py:   with lock: shared += 1
来源：http://bx.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://qd.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vh.panjiajie.cn

TS:   // 同 JS
来源：http://tp.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://re.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://si.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bm.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://yf.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ze.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://lu.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ym.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://pa.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mm.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ol.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wk.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wj.asd995.cn

C#:   async Task F() { await G(); }
来源：http://kg.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://ol.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://gr.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ut.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://yg.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://ub.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://be.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qu.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://zj.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mr.colortex.cn

[O06] 使用进程池
来源：http://ys.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sy.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bz.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://by.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://ck.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kc.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oc.yuexingan06.cn

Ruby: // fork 块
来源：http://vi.muxihuayi.cn

C#:   Parallel.For
来源：http://ud.yuntaijiaju.cn

================================================================================
来源：http://uh.nicolike.cn

P. 常用工具函数
来源：http://rs.shxzskj.cn

================================================================================
来源：http://mn.szxytkj.cn

[P01] 生成 UUID
来源：http://hj.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://wg.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lv.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://uo.9csxet.cn

TS:   crypto.randomUUID()
来源：http://by.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://lf.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ax.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://pc.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://mg.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://vz.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ug.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vl.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xs.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ho.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dx.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sc.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bk.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bd.newstarts.cn

[P03] 生成短随机字符串
来源：http://ap.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://au.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ir.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lh.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zv.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kn.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cf.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qa.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ra.521024.cn

[P04] 求长度
来源：http://lb.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mu.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ho.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kr.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ns.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://bb.colortex.cn

Go:   len(arr);  len(m)
来源：http://gs.shxzukj.cn

Ruby: x.length;  x.size
来源：http://gj.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bo.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://og.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lg.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vc.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ba.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ux.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pn.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sg.shtwfgs.cn

Ruby: a == b
来源：http://wg.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://so.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uv.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ny.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://ba.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dp.haigaiapp.cn

TS:   if (x == null) {}
来源：http://op.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nm.huixiangedu.cn

Go:   if x == nil {}
来源：http://qn.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ux.9csxet.cn

C#:   if (x is null) {}
来源：http://ac.muxihuayi.cn

[P07] 防抖与节流
来源：http://fq.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sf.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://kf.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pk.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://on.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://en.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pf.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://in.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ev.asd995.cn

[P08] 处理浮点精度问题
来源：http://en.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kv.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xi.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zu.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xp.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cl.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wy.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lr.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://el.szsharing.cn

================================================================================
来源：http://dm.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ye.huanxung.cn

================================================================================
来源：http://iv.jianghongdianzi.cn

[Q01] 创建表
来源：http://dt.gzmigu.cn

CREATE TABLE users (
来源：http://tn.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uh.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://pr.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://ly.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tr.haigaiapp.cn

);
来源：http://gx.nszjky.cn

[Q02] 创建带外键的表
来源：http://dj.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://wr.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ci.521024.cn

user_id INT NOT NULL,
来源：http://kl.hahajie.cn

amount DECIMAL(10, 2),
来源：http://ot.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mv.huanxung.cn

);
来源：http://cr.shxzskj.cn

[Q03] 增加列
来源：http://an.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mx.huixiangedu.cn

[Q04] 修改列类型
来源：http://gj.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dn.hnjuh.cn

[Q05] 重命名列
来源：http://ig.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ud.lnxyls.cn

[Q06] 删除列
来源：http://ss.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rb.huixinmuqiang.cn

[Q07] 删除表
来源：http://zt.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://bt.shxzskj.cn

[Q08] 创建普通索引
来源：http://no.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dv.szsharing.cn

[Q09] 创建唯一索引
来源：http://iw.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rn.jianghongdianzi.cn

[Q10] 插入单行
来源：http://jr.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pu.yuexingan06.cn

[Q11] 一次插入多行
来源：http://sw.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xn.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://fn.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sb.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rw.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://mt.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mz.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://rb.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wj.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zc.newstarts.cn

[Q15] 查询全部
来源：http://jq.nszjky.cn

SELECT * FROM users;
来源：http://qu.shxzukj.cn

[Q16] 查询指定列
来源：http://uy.shxzskj.cn

SELECT id, name FROM users;
来源：http://qd.lnxyls.cn

[Q17] 条件查询
来源：http://lc.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ic.9csxet.cn

[Q18] 模糊匹配
来源：http://oi.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zt.yuntaijiaju.cn

[Q19] 范围查询
来源：http://mu.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qp.panjiajie.cn

[Q20] IN 列表
来源：http://yj.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qg.haigaiapp.cn

[Q21] 空值判断
来源：http://ay.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://te.chemitech.net.cn

[Q22] 排序
来源：http://yu.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kt.szsharing.cn

[Q23] 分页
来源：http://po.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://df.jianghongdianzi.cn

[Q24] 去重
来源：http://gw.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://fm.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://yu.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://um.lnxyls.cn

[Q26] 计数
来源：http://rk.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ny.hnjuh.cn

[Q27] 条件计数
来源：http://ha.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fa.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://bb.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mg.newstarts.cn

[Q29] 最大最小值
来源：http://vl.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tq.gzmigu.cn

[Q30] 分组统计
来源：http://pi.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ps.szsharing.cn

[Q31] 分组后过滤
来源：http://yu.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yv.nicolike.cn

[Q32] 分组拼接字符串
来源：http://dr.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kt.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://he.newstarts.cn

[Q33] 多列分组
来源：http://gw.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ul.szxytkj.cn

[Q34] 每组取第一条
来源：http://hf.wgjwhj.cn

SELECT * FROM (
来源：http://na.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ht.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://yg.muxihuayi.cn

[Q35] 内连接
来源：http://ge.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vx.shxzukj.cn

[Q36] 左连接
来源：http://rm.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bz.nicolike.cn

[Q37] 右连接
来源：http://uk.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ax.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bk.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oj.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://cy.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bq.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oe.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ur.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yz.shtwfgs.cn

[Q41] 多表连接
来源：http://st.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nh.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://yo.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://ep.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://lr.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://at.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dw.shxzskj.cn

[Q43] 标量子查询
来源：http://sh.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xy.shxzskj.cn

[Q44] IN 子查询
来源：http://hs.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ha.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ft.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hc.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://im.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eb.asd995.cn

[Q47] 与平均值比较
来源：http://kz.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yp.asd995.cn

[Q48] CTE 公用表表达式
来源：http://wg.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pd.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://yy.yuexingan06.cn

[Q49] 更新单行
来源：http://ev.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fk.huixinmuqiang.cn

[Q50] 批量更新
来源：http://kv.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zc.asd995.cn

[Q51] 用子查询更新
来源：http://fi.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://md.jctech888.com.cn

[Q52] 删除指定行
来源：http://db.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://ko.shtwfgs.cn

[Q53] 按条件删除
来源：http://at.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mk.shtwfgs.cn

[Q54] 清空表
来源：http://sk.521024.cn

TRUNCATE TABLE logs;
来源：http://tx.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://ko.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hy.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://ta.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sa.bjjhwx.cn

[Q57] 行号
来源：http://fq.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ax.huixiangedu.cn

[Q58] 累计求和
来源：http://jm.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://si.bjjhwx.cn

[Q59] 分组内累计
来源：http://rq.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ab.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://tt.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oq.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sq.shxzukj.cn

[Q61] 移动平均
来源：http://ye.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bs.lnxyls.cn

[Q62] 分组占比
来源：http://gk.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ir.huixiangedu.cn

[Q63] 开启事务
来源：http://jd.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://op.colortex.cn

[Q64] 提交事务
来源：http://oi.jctech888.com.cn

COMMIT;
来源：http://jj.hnjuh.cn

[Q65] 回滚事务
来源：http://nq.szxytkj.cn

ROLLBACK;
来源：http://xt.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://lc.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kn.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://pb.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zv.chemitech.net.cn

[Q68] 保存点
来源：http://xd.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://zz.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://ez.szxytkj.cn

[Q69] 查看执行计划
来源：http://zf.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pt.szsharing.cn

[Q70] 更新统计信息
来源：http://mc.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://dd.wgjwhj.cn

[Q71] 查看建表语句
来源：http://bs.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qt.chemitech.net.cn

[Q72] 查看索引
来源：http://vp.newstarts.cn

SHOW INDEX FROM users;
来源：http://pa.szxytkj.cn

[Q73] 查看表状态
来源：http://oe.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cj.lnxyls.cn

[Q74] 强制使用索引
来源：http://pl.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kz.shxzukj.cn

[Q75] 日期格式化
来源：http://ln.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cd.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://va.huanxung.cn

[Q76] 按天统计
来源：http://lu.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wy.wgjwhj.cn

[Q77] 时间加减
来源：http://ed.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fn.jctech888.com.cn


<!-- 参考信息 -->