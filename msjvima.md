代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qj.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gs.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wx.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gz.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qi.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vf.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ub.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gl.jctech888.com.cn

================================================================================
来源：http://fp.lnxyls.cn

O. 并发与异步
来源：http://zh.shtwfgs.cn

================================================================================
来源：http://pr.newstarts.cn

[O01] 启动一个线程
来源：http://vm.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ui.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yz.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kr.huanxung.cn

TS:   // 同 JS
来源：http://oa.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://py.szxytkj.cn

Go:   go f()
来源：http://nb.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://jy.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://or.yuexingan06.cn

[O02] 使用线程池
来源：http://pn.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xq.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bz.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://rs.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://jd.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xz.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ck.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zt.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tv.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://de.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://ag.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://mp.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ws.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ql.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://lr.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xt.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kn.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://wi.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://dp.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://wx.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oy.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://fj.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oi.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dt.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cc.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bx.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://wc.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://jp.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://zq.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kj.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://pl.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://ep.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pn.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://my.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://cz.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rl.bjjhwx.cn

[O06] 使用进程池
来源：http://zf.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eq.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wn.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://bu.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://ug.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bs.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cq.panjiajie.cn

Ruby: // fork 块
来源：http://ba.yuexingan06.cn

C#:   Parallel.For
来源：http://ik.shtwfgs.cn

================================================================================
来源：http://bu.nszjky.cn

P. 常用工具函数
来源：http://vi.9csxet.cn

================================================================================
来源：http://un.haigaiapp.cn

[P01] 生成 UUID
来源：http://qr.colortex.cn

Py:   str(uuid.uuid4())
来源：http://hx.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ow.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://ii.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://nj.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://rv.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://bw.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://gq.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://wt.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://sv.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ot.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ge.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xr.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zb.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yk.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xu.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wf.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sx.panjiajie.cn

[P03] 生成短随机字符串
来源：http://zr.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oo.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xd.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ps.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fz.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jb.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mp.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xu.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ow.newstarts.cn

[P04] 求长度
来源：http://ca.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bg.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://op.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sy.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sd.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://ii.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://uj.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://vh.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cg.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://rw.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fo.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hp.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ct.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bf.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bv.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yb.wgjwhj.cn

Ruby: a == b
来源：http://gy.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jy.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sp.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://py.colortex.cn

PHP:  if (empty($x)) {}
来源：http://sp.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ku.haigaiapp.cn

TS:   if (x == null) {}
来源：http://yz.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hk.shxzukj.cn

Go:   if x == nil {}
来源：http://vw.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iv.yuexingan06.cn

C#:   if (x is null) {}
来源：http://gi.newstarts.cn

[P07] 防抖与节流
来源：http://pw.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xn.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://st.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ca.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xk.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bn.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nh.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oq.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://we.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://qv.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ya.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cp.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ad.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yy.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://je.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://au.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zk.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cx.shxzskj.cn

================================================================================
来源：http://wl.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://px.yuexingan06.cn

================================================================================
来源：http://nb.asd995.cn

[Q01] 创建表
来源：http://ec.lnxyls.cn

CREATE TABLE users (
来源：http://sr.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://by.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://rq.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://gz.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fi.huixinmuqiang.cn

);
来源：http://nv.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://pc.szxytkj.cn

CREATE TABLE orders (
来源：http://pb.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jv.hahajie.cn

user_id INT NOT NULL,
来源：http://ij.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://jn.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jh.panjiajie.cn

);
来源：http://uv.colortex.cn

[Q03] 增加列
来源：http://xd.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tt.huanxung.cn

[Q04] 修改列类型
来源：http://ux.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wu.shxzukj.cn

[Q05] 重命名列
来源：http://iq.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zw.muxihuayi.cn

[Q06] 删除列
来源：http://ae.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ps.nszjky.cn

[Q07] 删除表
来源：http://nc.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://us.newstarts.cn

[Q08] 创建普通索引
来源：http://kt.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fe.521024.cn

[Q09] 创建唯一索引
来源：http://in.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xy.chemitech.net.cn

[Q10] 插入单行
来源：http://gg.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jn.shxzskj.cn

[Q11] 一次插入多行
来源：http://ct.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rf.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://lu.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xl.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yn.shxzukj.cn

[Q13] 忽略重复插入
来源：http://hj.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mh.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://lz.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ep.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ud.panjiajie.cn

[Q15] 查询全部
来源：http://pn.chemitech.net.cn

SELECT * FROM users;
来源：http://hj.gzmigu.cn

[Q16] 查询指定列
来源：http://gy.shxzskj.cn

SELECT id, name FROM users;
来源：http://vd.hnjuh.cn

[Q17] 条件查询
来源：http://cj.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wr.shtwfgs.cn

[Q18] 模糊匹配
来源：http://zm.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dv.huixinmuqiang.cn

[Q19] 范围查询
来源：http://nu.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ka.asd995.cn

[Q20] IN 列表
来源：http://xu.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zb.haigaiapp.cn

[Q21] 空值判断
来源：http://lc.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hh.shtwfgs.cn

[Q22] 排序
来源：http://tq.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fu.huanxung.cn

[Q23] 分页
来源：http://ip.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hh.521024.cn

[Q24] 去重
来源：http://jp.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://fd.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://mj.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rc.521024.cn

[Q26] 计数
来源：http://xe.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://rb.chemitech.net.cn

[Q27] 条件计数
来源：http://jn.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jr.newstarts.cn

[Q28] 求和与平均
来源：http://qe.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lk.9csxet.cn

[Q29] 最大最小值
来源：http://lk.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iq.nszjky.cn

[Q30] 分组统计
来源：http://sm.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ox.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://kz.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ll.colortex.cn

[Q32] 分组拼接字符串
来源：http://iv.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yq.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://py.huanxung.cn

[Q33] 多列分组
来源：http://th.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://da.gzmigu.cn

[Q34] 每组取第一条
来源：http://yp.szxytkj.cn

SELECT * FROM (
来源：http://ze.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lh.nicolike.cn

) t WHERE rn = 1;
来源：http://li.szxytkj.cn

[Q35] 内连接
来源：http://ak.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cy.newstarts.cn

[Q36] 左连接
来源：http://nv.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ub.haigaiapp.cn

[Q37] 右连接
来源：http://xy.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xg.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://br.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://md.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://oh.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qd.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lt.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ts.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rr.muxihuayi.cn

[Q41] 多表连接
来源：http://nt.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://md.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://dk.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://jl.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://ls.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://ms.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cr.nszjky.cn

[Q43] 标量子查询
来源：http://zm.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ta.nicolike.cn

[Q44] IN 子查询
来源：http://fu.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sz.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://rg.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://no.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ut.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hu.hnjuh.cn

[Q47] 与平均值比较
来源：http://qs.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uq.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://kx.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tn.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://kj.panjiajie.cn

[Q49] 更新单行
来源：http://lv.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dj.newstarts.cn

[Q50] 批量更新
来源：http://uw.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ss.haigaiapp.cn

[Q51] 用子查询更新
来源：http://kk.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oh.jctech888.com.cn

[Q52] 删除指定行
来源：http://il.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://kg.asd995.cn

[Q53] 按条件删除
来源：http://gc.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ir.chemitech.net.cn

[Q54] 清空表
来源：http://bb.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://wd.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://qd.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dp.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://ak.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://se.szsharing.cn

[Q57] 行号
来源：http://ra.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sz.bjjhwx.cn

[Q58] 累计求和
来源：http://ma.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fl.shtwfgs.cn

[Q59] 分组内累计
来源：http://ya.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wj.521024.cn

[Q60] 取上一行 / 下一行
来源：http://bi.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jm.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jf.wgjwhj.cn

[Q61] 移动平均
来源：http://xz.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kn.hahajie.cn

[Q62] 分组占比
来源：http://za.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hn.gzmigu.cn

[Q63] 开启事务
来源：http://ed.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gq.shxzskj.cn

[Q64] 提交事务
来源：http://hc.huixinmuqiang.cn

COMMIT;
来源：http://hi.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://ca.gzmigu.cn

ROLLBACK;
来源：http://bj.hahajie.cn

[Q66] 行锁查询
来源：http://ab.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oo.newstarts.cn

[Q67] 设置隔离级别
来源：http://vq.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qv.chemitech.net.cn

[Q68] 保存点
来源：http://ku.lnxyls.cn

SAVEPOINT sp1;
来源：http://yh.521024.cn


<!-- 参考信息 -->