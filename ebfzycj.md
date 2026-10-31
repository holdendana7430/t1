代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://th.huanxung.cn

Go:   go f()
来源：http://rq.9csxet.cn

Ruby: Thread.new { f }
来源：http://zi.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://fl.shtwfgs.cn

[O02] 使用线程池
来源：http://ug.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ce.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rw.hahajie.cn

JS:   // worker_threads 线程池
来源：http://ht.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://to.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ad.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yt.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ty.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zd.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://lh.lnxyls.cn

Py:   with lock: shared += 1
来源：http://yc.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ts.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ua.colortex.cn

TS:   // 同 JS
来源：http://kd.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://bb.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vp.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vh.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://qb.nszjky.cn

[O04] 定义异步函数并等待
来源：http://ap.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://zf.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nd.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://tb.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ek.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cx.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xj.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ui.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://bi.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://ax.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://qu.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ig.asd995.cn

JS:   await Promise.all(tasks)
来源：http://oc.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://vl.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tl.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rt.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://am.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pj.jianghongdianzi.cn

[O06] 使用进程池
来源：http://af.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ra.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mx.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://lj.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://as.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nj.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qr.huixinmuqiang.cn

Ruby: // fork 块
来源：http://mu.chemitech.net.cn

C#:   Parallel.For
来源：http://wo.chemitech.net.cn

================================================================================
来源：http://uq.asd995.cn

P. 常用工具函数
来源：http://rd.bjjhwx.cn

================================================================================
来源：http://be.9csxet.cn

[P01] 生成 UUID
来源：http://rj.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ht.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bg.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://eq.9csxet.cn

TS:   crypto.randomUUID()
来源：http://fz.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://sd.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://an.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://nm.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://rq.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ff.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wn.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ee.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xv.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pd.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zi.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ye.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ws.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://la.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://xs.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bc.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sy.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wo.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vm.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hr.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ah.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zy.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zg.huanxung.cn

[P04] 求长度
来源：http://sh.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ma.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kn.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://um.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ka.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://cp.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://in.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://uo.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xr.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://tg.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zb.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://te.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ku.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tw.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oe.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dz.yuntaijiaju.cn

Ruby: a == b
来源：http://dx.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bz.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iu.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dr.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ob.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://do.szsharing.cn

TS:   if (x == null) {}
来源：http://um.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tv.huanxung.cn

Go:   if x == nil {}
来源：http://dg.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ar.haigaiapp.cn

C#:   if (x is null) {}
来源：http://rd.gzmigu.cn

[P07] 防抖与节流
来源：http://me.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sa.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ql.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dx.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tc.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pj.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wl.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vj.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oc.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://bu.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ud.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zl.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ct.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ag.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://il.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vg.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fq.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uh.panjiajie.cn

================================================================================
来源：http://ub.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xt.yuntaijiaju.cn

================================================================================
来源：http://uh.asd995.cn

[Q01] 创建表
来源：http://mp.jctech888.com.cn

CREATE TABLE users (
来源：http://gu.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sv.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://pw.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://qk.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iv.jctech888.com.cn

);
来源：http://lo.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://kw.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://wj.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sg.shxzskj.cn

user_id INT NOT NULL,
来源：http://ow.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://er.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dv.hnjuh.cn

);
来源：http://gc.shtwfgs.cn

[Q03] 增加列
来源：http://td.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uc.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://ci.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cr.asd995.cn

[Q05] 重命名列
来源：http://hr.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rt.bookmarksfly.cn

[Q06] 删除列
来源：http://pq.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ax.jianghongdianzi.cn

[Q07] 删除表
来源：http://aw.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ay.wgjwhj.cn

[Q08] 创建普通索引
来源：http://if.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xn.hahajie.cn

[Q09] 创建唯一索引
来源：http://sc.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jh.haigaiapp.cn

[Q10] 插入单行
来源：http://vp.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ny.jctech888.com.cn

[Q11] 一次插入多行
来源：http://bv.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lb.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://dt.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pq.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ws.shxzukj.cn

[Q13] 忽略重复插入
来源：http://yl.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gu.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://fs.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fu.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yu.huixinmuqiang.cn

[Q15] 查询全部
来源：http://rj.panjiajie.cn

SELECT * FROM users;
来源：http://mo.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://ha.haigaiapp.cn

SELECT id, name FROM users;
来源：http://bp.gzmigu.cn

[Q17] 条件查询
来源：http://wf.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xx.shxzukj.cn

[Q18] 模糊匹配
来源：http://mw.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qe.hahajie.cn

[Q19] 范围查询
来源：http://vn.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fx.shxzukj.cn

[Q20] IN 列表
来源：http://sn.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ft.shxzskj.cn

[Q21] 空值判断
来源：http://tn.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kz.muxihuayi.cn

[Q22] 排序
来源：http://ge.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lc.szxytkj.cn

[Q23] 分页
来源：http://na.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kx.szxytkj.cn

[Q24] 去重
来源：http://gc.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://ig.9csxet.cn

[Q25] 只取前 N 条
来源：http://iu.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ge.nszjky.cn

[Q26] 计数
来源：http://om.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://po.jianghongdianzi.cn

[Q27] 条件计数
来源：http://tv.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yy.haigaiapp.cn

[Q28] 求和与平均
来源：http://by.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cm.hnjuh.cn

[Q29] 最大最小值
来源：http://nu.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ts.9csxet.cn

[Q30] 分组统计
来源：http://va.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wv.nicolike.cn

[Q31] 分组后过滤
来源：http://zs.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xa.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://fp.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mr.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mh.huixinmuqiang.cn

[Q33] 多列分组
来源：http://fl.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cg.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://fn.shxzukj.cn

SELECT * FROM (
来源：http://ch.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xc.huixiangedu.cn

) t WHERE rn = 1;
来源：http://om.lnxyls.cn

[Q35] 内连接
来源：http://yk.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xi.chemitech.net.cn

[Q36] 左连接
来源：http://me.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nk.shtwfgs.cn

[Q37] 右连接
来源：http://pj.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qk.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ud.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mu.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://mb.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wi.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uy.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ki.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://we.asd995.cn

[Q41] 多表连接
来源：http://aj.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yh.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://eh.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://jr.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://we.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://sy.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vr.lnxyls.cn

[Q43] 标量子查询
来源：http://uv.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vi.wgjwhj.cn

[Q44] IN 子查询
来源：http://wj.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sw.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://wc.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rk.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zk.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://es.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://rn.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://up.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://tn.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hj.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://da.shxzskj.cn

[Q49] 更新单行
来源：http://sz.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vv.521024.cn

[Q50] 批量更新
来源：http://fi.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cz.jctech888.com.cn

[Q51] 用子查询更新
来源：http://kp.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jc.muxihuayi.cn

[Q52] 删除指定行
来源：http://aw.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://sy.shxzukj.cn

[Q53] 按条件删除
来源：http://kx.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://is.panjiajie.cn

[Q54] 清空表
来源：http://xp.521024.cn

TRUNCATE TABLE logs;
来源：http://hp.nicolike.cn

[Q55] 排名（并列占位）
来源：http://nh.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kt.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://cj.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iq.huanxung.cn

[Q57] 行号
来源：http://az.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wd.shxzskj.cn

[Q58] 累计求和
来源：http://xn.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ny.wgjwhj.cn

[Q59] 分组内累计
来源：http://nx.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xx.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://ox.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ln.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jo.huanxung.cn

[Q61] 移动平均
来源：http://xz.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cl.shxzukj.cn

[Q62] 分组占比
来源：http://di.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fl.nicolike.cn

[Q63] 开启事务
来源：http://vi.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zm.wgjwhj.cn

[Q64] 提交事务
来源：http://hj.hahajie.cn

COMMIT;
来源：http://aj.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://sm.521024.cn

ROLLBACK;
来源：http://uk.chemitech.net.cn

[Q66] 行锁查询
来源：http://zy.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cf.9csxet.cn

[Q67] 设置隔离级别
来源：http://ku.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oq.muxihuayi.cn

[Q68] 保存点
来源：http://gv.szsharing.cn

SAVEPOINT sp1;
来源：http://pq.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://tf.shtwfgs.cn

[Q69] 查看执行计划
来源：http://ac.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fv.lnxyls.cn

[Q70] 更新统计信息
来源：http://np.gzmigu.cn

ANALYZE TABLE users;
来源：http://md.bjjhwx.cn

[Q71] 查看建表语句
来源：http://iw.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ik.szsharing.cn

[Q72] 查看索引
来源：http://am.szsharing.cn

SHOW INDEX FROM users;
来源：http://vh.9csxet.cn

[Q73] 查看表状态
来源：http://yo.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wp.jctech888.com.cn

[Q74] 强制使用索引
来源：http://bd.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sv.colortex.cn

[Q75] 日期格式化
来源：http://ke.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gm.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://se.bookmarksfly.cn


<!-- 参考信息 -->