代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dy.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fg.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://my.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ae.szsharing.cn

================================================================================
来源：http://ji.haigaiapp.cn

O. 并发与异步
来源：http://cf.panjiajie.cn

================================================================================
来源：http://yo.huixiangedu.cn

[O01] 启动一个线程
来源：http://cs.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://za.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://st.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ka.yuexingan06.cn

TS:   // 同 JS
来源：http://wf.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://hn.521024.cn

Go:   go f()
来源：http://co.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://pt.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://vd.szsharing.cn

[O02] 使用线程池
来源：http://ao.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://li.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gi.521024.cn

JS:   // worker_threads 线程池
来源：http://dm.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://px.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nv.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zk.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rn.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fd.huanxung.cn

[O03] 加锁保护共享数据
来源：http://zp.gzmigu.cn

Py:   with lock: shared += 1
来源：http://rw.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://ns.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nm.asd995.cn

TS:   // 同 JS
来源：http://oe.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://ie.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uz.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wg.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://sw.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ko.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://oo.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ah.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://km.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vb.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jm.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tm.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://io.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://yu.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://dg.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://ml.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gq.521024.cn

JS:   await Promise.all(tasks)
来源：http://vb.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://mz.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iz.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iz.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://aa.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rv.nszjky.cn

[O06] 使用进程池
来源：http://zf.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xa.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kv.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://vz.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://do.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ey.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kl.521024.cn

Ruby: // fork 块
来源：http://xx.hnjuh.cn

C#:   Parallel.For
来源：http://to.muxihuayi.cn

================================================================================
来源：http://tj.yuexingan06.cn

P. 常用工具函数
来源：http://bs.gzmigu.cn

================================================================================
来源：http://zo.bookmarksfly.cn

[P01] 生成 UUID
来源：http://dm.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://la.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lf.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://wb.hahajie.cn

TS:   crypto.randomUUID()
来源：http://kp.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://pa.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://yz.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://pg.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://fc.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://op.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wh.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://or.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wo.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gy.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fy.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oa.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xn.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lz.panjiajie.cn

[P03] 生成短随机字符串
来源：http://pd.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bn.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cl.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zl.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lg.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jt.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mg.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ih.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tv.haigaiapp.cn

[P04] 求长度
来源：http://ik.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bx.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gn.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jd.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://we.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://xy.szsharing.cn

Go:   len(arr);  len(m)
来源：http://js.nszjky.cn

Ruby: x.length;  x.size
来源：http://kp.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://is.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://yj.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jb.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://us.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ic.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gd.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ou.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mm.gzmigu.cn

Ruby: a == b
来源：http://ty.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fx.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gj.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jh.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://np.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ea.521024.cn

TS:   if (x == null) {}
来源：http://ic.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ob.muxihuayi.cn

Go:   if x == nil {}
来源：http://vk.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://is.szxytkj.cn

C#:   if (x is null) {}
来源：http://mp.asd995.cn

[P07] 防抖与节流
来源：http://of.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zi.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://np.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bg.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ls.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://da.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gw.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wk.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ls.nszjky.cn

[P08] 处理浮点精度问题
来源：http://nj.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kc.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hn.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tl.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nn.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xh.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xp.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ey.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oi.bjjhwx.cn

================================================================================
来源：http://cd.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iw.lnxyls.cn

================================================================================
来源：http://zv.shxzukj.cn

[Q01] 创建表
来源：http://fc.nszjky.cn

CREATE TABLE users (
来源：http://fa.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mg.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ly.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://fq.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ut.bookmarksfly.cn

);
来源：http://vs.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://rv.bookmarksfly.cn

CREATE TABLE orders (
来源：http://vl.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ow.huixiangedu.cn

user_id INT NOT NULL,
来源：http://yx.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://bq.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jt.nszjky.cn

);
来源：http://ev.9csxet.cn

[Q03] 增加列
来源：http://kz.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uz.gzmigu.cn

[Q04] 修改列类型
来源：http://md.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rp.shxzukj.cn

[Q05] 重命名列
来源：http://ty.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oe.9csxet.cn

[Q06] 删除列
来源：http://qq.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hj.shtwfgs.cn

[Q07] 删除表
来源：http://pm.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://li.nicolike.cn

[Q08] 创建普通索引
来源：http://df.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cf.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ds.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://se.bookmarksfly.cn

[Q10] 插入单行
来源：http://qo.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yw.huanxung.cn

[Q11] 一次插入多行
来源：http://jk.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ww.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://jm.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://um.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sb.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://op.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ok.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://tq.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ed.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gi.colortex.cn

[Q15] 查询全部
来源：http://ti.muxihuayi.cn

SELECT * FROM users;
来源：http://xx.hnjuh.cn

[Q16] 查询指定列
来源：http://ye.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://tg.jianghongdianzi.cn

[Q17] 条件查询
来源：http://jb.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ti.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://by.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kr.haigaiapp.cn

[Q19] 范围查询
来源：http://mo.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vu.asd995.cn

[Q20] IN 列表
来源：http://yb.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pk.hnjuh.cn

[Q21] 空值判断
来源：http://js.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nm.hnjuh.cn

[Q22] 排序
来源：http://ho.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ny.hnjuh.cn

[Q23] 分页
来源：http://ul.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ko.nszjky.cn

[Q24] 去重
来源：http://gk.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://bh.lnxyls.cn

[Q25] 只取前 N 条
来源：http://pm.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://id.bjjhwx.cn

[Q26] 计数
来源：http://fq.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://bd.nszjky.cn

[Q27] 条件计数
来源：http://uh.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://im.szsharing.cn

[Q28] 求和与平均
来源：http://vj.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://er.nicolike.cn

[Q29] 最大最小值
来源：http://dj.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cq.szxytkj.cn

[Q30] 分组统计
来源：http://xf.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yz.hnjuh.cn

[Q31] 分组后过滤
来源：http://he.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mz.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://ct.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sc.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qd.9csxet.cn

[Q33] 多列分组
来源：http://ei.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tg.hnjuh.cn

[Q34] 每组取第一条
来源：http://yv.haigaiapp.cn

SELECT * FROM (
来源：http://lf.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zr.newstarts.cn

) t WHERE rn = 1;
来源：http://rx.haigaiapp.cn

[Q35] 内连接
来源：http://sa.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eo.shtwfgs.cn

[Q36] 左连接
来源：http://mm.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ft.jctech888.com.cn

[Q37] 右连接
来源：http://jq.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://on.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bu.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xk.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ex.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zf.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fp.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://if.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zi.huixinmuqiang.cn

[Q41] 多表连接
来源：http://oj.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bs.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://en.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://lo.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://oe.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://br.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zu.jctech888.com.cn

[Q43] 标量子查询
来源：http://gh.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qo.shxzskj.cn

[Q44] IN 子查询
来源：http://yd.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ja.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://fr.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rh.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xn.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ms.shtwfgs.cn

[Q47] 与平均值比较
来源：http://en.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://be.colortex.cn

[Q48] CTE 公用表表达式
来源：http://mz.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nc.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://bu.huanxung.cn

[Q49] 更新单行
来源：http://hy.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://az.9csxet.cn

[Q50] 批量更新
来源：http://wz.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://is.gzmigu.cn

[Q51] 用子查询更新
来源：http://sw.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mx.chemitech.net.cn

[Q52] 删除指定行
来源：http://ai.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://ad.panjiajie.cn

[Q53] 按条件删除
来源：http://gj.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iv.nicolike.cn

[Q54] 清空表
来源：http://ij.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://ka.szsharing.cn

[Q55] 排名（并列占位）
来源：http://ni.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gd.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ph.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rw.9csxet.cn

[Q57] 行号
来源：http://gj.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sm.521024.cn

[Q58] 累计求和
来源：http://aa.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fj.nicolike.cn

[Q59] 分组内累计
来源：http://vm.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hw.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ow.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zx.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ov.jctech888.com.cn

[Q61] 移动平均
来源：http://ao.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xb.chemitech.net.cn

[Q62] 分组占比
来源：http://he.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pa.521024.cn

[Q63] 开启事务
来源：http://vu.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cw.bookmarksfly.cn

[Q64] 提交事务
来源：http://bi.colortex.cn

COMMIT;
来源：http://ku.9csxet.cn

[Q65] 回滚事务
来源：http://dr.huanxung.cn

ROLLBACK;
来源：http://rs.wgjwhj.cn

[Q66] 行锁查询
来源：http://hl.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cx.gzmigu.cn

[Q67] 设置隔离级别
来源：http://cx.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dj.muxihuayi.cn

[Q68] 保存点
来源：http://vw.shxzukj.cn

SAVEPOINT sp1;
来源：http://xb.521024.cn

ROLLBACK TO sp1;
来源：http://cq.shtwfgs.cn

[Q69] 查看执行计划
来源：http://jd.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gw.nszjky.cn

[Q70] 更新统计信息
来源：http://rd.haigaiapp.cn


<!-- 参考信息 -->