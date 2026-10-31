代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fo.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mh.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tr.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dz.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sh.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mo.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pf.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nr.jianghongdianzi.cn

================================================================================
来源：http://pw.lnxyls.cn

O. 并发与异步
来源：http://vf.jctech888.com.cn

================================================================================
来源：http://bk.shtwfgs.cn

[O01] 启动一个线程
来源：http://fq.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kw.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hk.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iz.wgjwhj.cn

TS:   // 同 JS
来源：http://ed.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://dw.lnxyls.cn

Go:   go f()
来源：http://hu.asd995.cn

Ruby: Thread.new { f }
来源：http://wt.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://km.szsharing.cn

[O02] 使用线程池
来源：http://xz.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dy.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qh.nszjky.cn

JS:   // worker_threads 线程池
来源：http://yo.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://uv.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ve.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://us.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ne.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iw.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://uu.shxzskj.cn

Py:   with lock: shared += 1
来源：http://ty.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://si.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zo.shxzukj.cn

TS:   // 同 JS
来源：http://wy.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://wq.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dv.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://md.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://gp.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://hs.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://xb.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rg.9csxet.cn

JS:   async function f() { await g(); }
来源：http://gq.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vf.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fz.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oe.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tq.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://co.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://zg.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://hf.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://le.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://gj.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://zb.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mt.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vh.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ah.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hj.huanxung.cn

[O06] 使用进程池
来源：http://mo.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ve.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ae.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://bl.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://wu.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gp.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rd.jctech888.com.cn

Ruby: // fork 块
来源：http://te.521024.cn

C#:   Parallel.For
来源：http://tj.huixiangedu.cn

================================================================================
来源：http://dn.hahajie.cn

P. 常用工具函数
来源：http://mn.newstarts.cn

================================================================================
来源：http://qa.yuexingan06.cn

[P01] 生成 UUID
来源：http://mx.521024.cn

Py:   str(uuid.uuid4())
来源：http://rs.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ws.nicolike.cn

JS:   crypto.randomUUID()
来源：http://zc.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://tx.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://wl.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://fn.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://ve.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://mq.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://ls.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rh.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ge.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tv.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://br.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zt.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aw.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gz.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vi.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://rg.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yt.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zh.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ni.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wf.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yo.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://og.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gj.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qj.nszjky.cn

[P04] 求长度
来源：http://du.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hj.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qq.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://me.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bn.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://pa.hahajie.cn

Go:   len(arr);  len(m)
来源：http://vu.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ho.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pa.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://hx.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ff.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gl.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kh.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rd.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oj.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yj.asd995.cn

Ruby: a == b
来源：http://as.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lf.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uk.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oq.521024.cn

PHP:  if (empty($x)) {}
来源：http://hf.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pe.shxzukj.cn

TS:   if (x == null) {}
来源：http://mq.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kn.newstarts.cn

Go:   if x == nil {}
来源：http://hu.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hr.bjjhwx.cn

C#:   if (x is null) {}
来源：http://br.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ww.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ar.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://as.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ds.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qy.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rd.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qw.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ct.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tv.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://dn.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://na.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://df.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xf.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ga.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pz.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ch.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qm.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yj.szsharing.cn

================================================================================
来源：http://ie.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zb.newstarts.cn

================================================================================
来源：http://ga.muxihuayi.cn

[Q01] 创建表
来源：http://hk.colortex.cn

CREATE TABLE users (
来源：http://pf.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nj.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://yk.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://ue.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rs.chemitech.net.cn

);
来源：http://cs.panjiajie.cn

[Q02] 创建带外键的表
来源：http://zi.haigaiapp.cn

CREATE TABLE orders (
来源：http://px.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ca.shxzukj.cn

user_id INT NOT NULL,
来源：http://lt.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://mm.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://et.shxzskj.cn

);
来源：http://ap.hnjuh.cn

[Q03] 增加列
来源：http://im.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eq.bookmarksfly.cn

[Q04] 修改列类型
来源：http://aq.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nr.asd995.cn

[Q05] 重命名列
来源：http://qw.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ma.hnjuh.cn

[Q06] 删除列
来源：http://od.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qs.panjiajie.cn

[Q07] 删除表
来源：http://yc.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://rg.panjiajie.cn

[Q08] 创建普通索引
来源：http://dw.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ht.asd995.cn

[Q09] 创建唯一索引
来源：http://pa.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wa.muxihuayi.cn

[Q10] 插入单行
来源：http://ua.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ft.muxihuayi.cn

[Q11] 一次插入多行
来源：http://hd.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lb.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://sk.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oj.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xr.colortex.cn

[Q13] 忽略重复插入
来源：http://pd.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xt.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://xg.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://th.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mi.hahajie.cn

[Q15] 查询全部
来源：http://hs.yuntaijiaju.cn

SELECT * FROM users;
来源：http://fk.bookmarksfly.cn

[Q16] 查询指定列
来源：http://cy.asd995.cn

SELECT id, name FROM users;
来源：http://of.shtwfgs.cn

[Q17] 条件查询
来源：http://gt.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://es.wgjwhj.cn

[Q18] 模糊匹配
来源：http://bd.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mf.hahajie.cn

[Q19] 范围查询
来源：http://ae.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lf.panjiajie.cn

[Q20] IN 列表
来源：http://qd.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gp.szxytkj.cn

[Q21] 空值判断
来源：http://iu.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yo.hnjuh.cn

[Q22] 排序
来源：http://ry.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ec.asd995.cn

[Q23] 分页
来源：http://ev.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://en.521024.cn

[Q24] 去重
来源：http://jt.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://cr.lnxyls.cn

[Q25] 只取前 N 条
来源：http://ct.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qz.haigaiapp.cn

[Q26] 计数
来源：http://pe.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://ps.muxihuayi.cn

[Q27] 条件计数
来源：http://rh.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ju.nszjky.cn

[Q28] 求和与平均
来源：http://sh.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yk.huanxung.cn

[Q29] 最大最小值
来源：http://rk.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hl.yuntaijiaju.cn

[Q30] 分组统计
来源：http://qj.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lp.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://nk.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kr.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://nt.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bq.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yz.chemitech.net.cn

[Q33] 多列分组
来源：http://yq.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tj.hahajie.cn

[Q34] 每组取第一条
来源：http://bu.huanxung.cn

SELECT * FROM (
来源：http://ge.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cw.wgjwhj.cn

) t WHERE rn = 1;
来源：http://ll.bjjhwx.cn

[Q35] 内连接
来源：http://sf.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://om.yuexingan06.cn

[Q36] 左连接
来源：http://vt.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zs.9csxet.cn

[Q37] 右连接
来源：http://xg.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iq.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ge.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kp.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://qx.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sm.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mc.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sq.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zo.gzmigu.cn

[Q41] 多表连接
来源：http://nj.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qh.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ps.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://bc.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://qa.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://ay.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mx.gzmigu.cn

[Q43] 标量子查询
来源：http://qy.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gj.shtwfgs.cn

[Q44] IN 子查询
来源：http://aj.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rf.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://gw.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ou.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wp.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tx.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://nq.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pg.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://aj.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://km.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://gn.bjjhwx.cn

[Q49] 更新单行
来源：http://zj.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ic.hnjuh.cn

[Q50] 批量更新
来源：http://jt.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dw.521024.cn

[Q51] 用子查询更新
来源：http://gr.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gq.chemitech.net.cn

[Q52] 删除指定行
来源：http://wd.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://xd.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://bc.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lv.panjiajie.cn

[Q54] 清空表
来源：http://ta.newstarts.cn

TRUNCATE TABLE logs;
来源：http://bq.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://ri.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rg.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://vz.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wu.shtwfgs.cn

[Q57] 行号
来源：http://wc.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cr.panjiajie.cn

[Q58] 累计求和
来源：http://ie.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nh.hnjuh.cn

[Q59] 分组内累计
来源：http://eo.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uf.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ev.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://th.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://te.521024.cn

[Q61] 移动平均
来源：http://ms.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jv.gzmigu.cn

[Q62] 分组占比
来源：http://gg.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cv.shxzskj.cn

[Q63] 开启事务
来源：http://vg.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://if.yuexingan06.cn

[Q64] 提交事务
来源：http://re.chemitech.net.cn

COMMIT;
来源：http://xa.szxytkj.cn

[Q65] 回滚事务
来源：http://bt.huanxung.cn

ROLLBACK;
来源：http://er.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://ik.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tj.asd995.cn

[Q67] 设置隔离级别
来源：http://un.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qg.yuexingan06.cn

[Q68] 保存点
来源：http://tl.szsharing.cn

SAVEPOINT sp1;
来源：http://iz.bookmarksfly.cn


<!-- 参考信息 -->