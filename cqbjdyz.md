代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://px.nszjky.cn

Go:   go f()
来源：http://ya.521024.cn

Ruby: Thread.new { f }
来源：http://dd.521024.cn

C#:   Task.Run(() => F());
来源：http://no.jianghongdianzi.cn

[O02] 使用线程池
来源：http://lt.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yx.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xm.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://gj.huanxung.cn

TS:   // worker_threads 线程池
来源：http://jt.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lb.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uv.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yo.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nt.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ew.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://cb.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://us.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://et.newstarts.cn

TS:   // 同 JS
来源：http://co.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://yo.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eq.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://at.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://pp.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://ci.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://th.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jb.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ds.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ko.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://js.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://io.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qm.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://ba.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://yg.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://ho.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://px.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://zj.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://nm.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tg.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://le.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ty.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://th.521024.cn

[O06] 使用进程池
来源：http://po.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ed.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mt.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://hd.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://rb.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ha.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ll.yuntaijiaju.cn

Ruby: // fork 块
来源：http://lp.asd995.cn

C#:   Parallel.For
来源：http://sb.huanxung.cn

================================================================================
来源：http://qt.asd995.cn

P. 常用工具函数
来源：http://bh.panjiajie.cn

================================================================================
来源：http://or.hahajie.cn

[P01] 生成 UUID
来源：http://lz.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://zl.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tg.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://eh.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://yf.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://uj.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://xd.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://vi.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wm.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://ns.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jf.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eu.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tn.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bc.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sb.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fv.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rr.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xx.nszjky.cn

[P03] 生成短随机字符串
来源：http://nu.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wo.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rx.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sf.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://go.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zf.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mb.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uh.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://as.wgjwhj.cn

[P04] 求长度
来源：http://qq.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nd.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wt.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pm.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kd.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://qw.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://tx.hahajie.cn

Ruby: x.length;  x.size
来源：http://uu.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://da.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://wk.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kc.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rj.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oe.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mo.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qt.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eo.jctech888.com.cn

Ruby: a == b
来源：http://rr.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qv.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yo.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tu.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://oo.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nv.hahajie.cn

TS:   if (x == null) {}
来源：http://gw.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iu.haigaiapp.cn

Go:   if x == nil {}
来源：http://dt.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oa.shxzukj.cn

C#:   if (x is null) {}
来源：http://ae.newstarts.cn

[P07] 防抖与节流
来源：http://xm.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tn.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://fk.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xh.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cy.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kr.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tf.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uo.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yw.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://na.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://df.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mm.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vj.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cy.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yr.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pj.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ra.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mc.szxytkj.cn

================================================================================
来源：http://rl.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yp.521024.cn

================================================================================
来源：http://xr.shtwfgs.cn

[Q01] 创建表
来源：http://dn.szsharing.cn

CREATE TABLE users (
来源：http://dc.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qf.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://np.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://ft.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ea.gzmigu.cn

);
来源：http://dl.panjiajie.cn

[Q02] 创建带外键的表
来源：http://na.hahajie.cn

CREATE TABLE orders (
来源：http://bi.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cl.shxzukj.cn

user_id INT NOT NULL,
来源：http://wt.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://tt.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qr.shxzukj.cn

);
来源：http://xk.nicolike.cn

[Q03] 增加列
来源：http://yi.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jh.huixiangedu.cn

[Q04] 修改列类型
来源：http://yy.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://if.huixiangedu.cn

[Q05] 重命名列
来源：http://eb.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xn.newstarts.cn

[Q06] 删除列
来源：http://zz.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nk.jianghongdianzi.cn

[Q07] 删除表
来源：http://nn.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://qx.chemitech.net.cn

[Q08] 创建普通索引
来源：http://fg.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bk.shxzskj.cn

[Q09] 创建唯一索引
来源：http://ri.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ep.asd995.cn

[Q10] 插入单行
来源：http://rj.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xi.gzmigu.cn

[Q11] 一次插入多行
来源：http://ro.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ua.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://gn.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ey.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qq.521024.cn

[Q13] 忽略重复插入
来源：http://oh.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xt.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://cy.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cl.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lf.521024.cn

[Q15] 查询全部
来源：http://rm.szxytkj.cn

SELECT * FROM users;
来源：http://cu.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://sb.bjjhwx.cn

SELECT id, name FROM users;
来源：http://dr.yuexingan06.cn

[Q17] 条件查询
来源：http://fu.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gj.521024.cn

[Q18] 模糊匹配
来源：http://nh.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mj.bjjhwx.cn

[Q19] 范围查询
来源：http://zn.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rp.hnjuh.cn

[Q20] IN 列表
来源：http://pm.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kq.newstarts.cn

[Q21] 空值判断
来源：http://li.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fc.lnxyls.cn

[Q22] 排序
来源：http://ql.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pi.wgjwhj.cn

[Q23] 分页
来源：http://hs.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ge.panjiajie.cn

[Q24] 去重
来源：http://yv.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://ly.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://si.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ga.haigaiapp.cn

[Q26] 计数
来源：http://pq.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://si.chemitech.net.cn

[Q27] 条件计数
来源：http://hl.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zg.hahajie.cn

[Q28] 求和与平均
来源：http://kh.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ig.szsharing.cn

[Q29] 最大最小值
来源：http://zt.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ne.lnxyls.cn

[Q30] 分组统计
来源：http://ue.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ym.shxzskj.cn

[Q31] 分组后过滤
来源：http://nm.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dk.szsharing.cn

[Q32] 分组拼接字符串
来源：http://iy.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yg.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ug.haigaiapp.cn

[Q33] 多列分组
来源：http://iu.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ao.panjiajie.cn

[Q34] 每组取第一条
来源：http://jb.521024.cn

SELECT * FROM (
来源：http://sn.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xd.haigaiapp.cn

) t WHERE rn = 1;
来源：http://az.hnjuh.cn

[Q35] 内连接
来源：http://mg.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uo.nicolike.cn

[Q36] 左连接
来源：http://cb.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ra.huixinmuqiang.cn

[Q37] 右连接
来源：http://yi.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mo.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lv.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ls.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://nd.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://np.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ta.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ph.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zc.lnxyls.cn

[Q41] 多表连接
来源：http://fm.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zy.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://lu.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://bu.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://zt.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://nu.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rq.521024.cn

[Q43] 标量子查询
来源：http://ls.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nv.nszjky.cn

[Q44] IN 子查询
来源：http://de.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kr.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://ol.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oc.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sb.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mu.wgjwhj.cn

[Q47] 与平均值比较
来源：http://xo.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qu.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://xs.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://to.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://qo.szsharing.cn

[Q49] 更新单行
来源：http://fc.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cp.panjiajie.cn

[Q50] 批量更新
来源：http://zs.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tq.colortex.cn

[Q51] 用子查询更新
来源：http://hc.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vr.asd995.cn

[Q52] 删除指定行
来源：http://ak.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://fy.yuexingan06.cn

[Q53] 按条件删除
来源：http://qu.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ed.asd995.cn

[Q54] 清空表
来源：http://qd.hahajie.cn

TRUNCATE TABLE logs;
来源：http://my.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://xr.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pt.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://ms.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hq.colortex.cn

[Q57] 行号
来源：http://jb.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xl.wgjwhj.cn

[Q58] 累计求和
来源：http://df.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wb.521024.cn

[Q59] 分组内累计
来源：http://ov.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cx.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://hp.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ty.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kd.szsharing.cn

[Q61] 移动平均
来源：http://ak.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nt.9csxet.cn

[Q62] 分组占比
来源：http://vg.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qx.wgjwhj.cn

[Q63] 开启事务
来源：http://ez.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kj.asd995.cn

[Q64] 提交事务
来源：http://vx.yuexingan06.cn

COMMIT;
来源：http://kn.colortex.cn

[Q65] 回滚事务
来源：http://tb.wgjwhj.cn

ROLLBACK;
来源：http://ey.asd995.cn

[Q66] 行锁查询
来源：http://fn.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nn.nicolike.cn

[Q67] 设置隔离级别
来源：http://qg.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ri.lnxyls.cn

[Q68] 保存点
来源：http://ri.panjiajie.cn

SAVEPOINT sp1;
来源：http://ka.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://yw.shxzskj.cn

[Q69] 查看执行计划
来源：http://rg.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sd.colortex.cn

[Q70] 更新统计信息
来源：http://ei.muxihuayi.cn

ANALYZE TABLE users;
来源：http://ud.nszjky.cn

[Q71] 查看建表语句
来源：http://iu.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://up.hahajie.cn

[Q72] 查看索引
来源：http://xz.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://ew.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://dm.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uk.jctech888.com.cn

[Q74] 强制使用索引
来源：http://xb.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rh.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://jc.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dg.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nz.jctech888.com.cn


<!-- 参考信息 -->