代发 wailian999

Go:   // 手写递归
来源：http://ku.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mp.yuexingan06.cn

C#:   // 手写递归
来源：http://ca.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fx.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zp.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cm.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gg.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zz.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ng.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tg.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hs.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qx.gzmigu.cn

================================================================================
来源：http://ml.huixiangedu.cn

O. 并发与异步
来源：http://ni.yuexingan06.cn

================================================================================
来源：http://ke.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://rv.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xs.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mo.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lf.hahajie.cn

TS:   // 同 JS
来源：http://xj.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://sc.yuntaijiaju.cn

Go:   go f()
来源：http://cy.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://wh.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://kq.huanxung.cn

[O02] 使用线程池
来源：http://xk.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ox.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://np.nicolike.cn

JS:   // worker_threads 线程池
来源：http://yc.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://xr.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uk.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://np.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vz.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://av.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://vr.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://zb.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ko.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ln.huixiangedu.cn

TS:   // 同 JS
来源：http://sa.521024.cn

Java: synchronized (this) { shared++; }
来源：http://al.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fq.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wi.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://jw.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://mb.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://uy.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://me.huanxung.cn

JS:   async function f() { await g(); }
来源：http://pf.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ui.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lj.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ww.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fd.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://zt.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://vu.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://gv.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bh.colortex.cn

JS:   await Promise.all(tasks)
来源：http://kx.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://di.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nz.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://as.asd995.cn

Ruby: threads.map(&:join)
来源：http://gx.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zo.haigaiapp.cn

[O06] 使用进程池
来源：http://qp.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hh.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zm.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://mk.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://ac.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mo.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://at.muxihuayi.cn

Ruby: // fork 块
来源：http://vj.hahajie.cn

C#:   Parallel.For
来源：http://jn.lnxyls.cn

================================================================================
来源：http://sz.shtwfgs.cn

P. 常用工具函数
来源：http://uk.szsharing.cn

================================================================================
来源：http://iw.colortex.cn

[P01] 生成 UUID
来源：http://ql.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://ju.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nc.colortex.cn

JS:   crypto.randomUUID()
来源：http://qg.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://bf.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://qy.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://nh.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://vc.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://ze.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://mh.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wx.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ss.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eg.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ns.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://om.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dj.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://to.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dg.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://hi.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fs.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oo.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cc.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://an.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cw.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dh.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ot.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cj.shxzskj.cn

[P04] 求长度
来源：http://rg.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xr.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xr.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xr.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kv.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://xj.newstarts.cn

Go:   len(arr);  len(m)
来源：http://lo.huanxung.cn

Ruby: x.length;  x.size
来源：http://xc.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xj.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://zr.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lh.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xf.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qf.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jb.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lo.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zx.yuntaijiaju.cn

Ruby: a == b
来源：http://yy.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dw.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ek.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rt.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://iq.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bo.shxzukj.cn

TS:   if (x == null) {}
来源：http://cw.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vy.bookmarksfly.cn

Go:   if x == nil {}
来源：http://ee.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ay.szsharing.cn

C#:   if (x is null) {}
来源：http://px.521024.cn

[P07] 防抖与节流
来源：http://xz.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://we.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://pj.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://td.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hx.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yj.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ov.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wf.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nl.nicolike.cn

[P08] 处理浮点精度问题
来源：http://wt.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cq.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vn.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yz.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eg.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ij.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://in.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pe.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zh.szxytkj.cn

================================================================================
来源：http://ij.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://na.huixiangedu.cn

================================================================================
来源：http://qb.shtwfgs.cn

[Q01] 创建表
来源：http://rc.jianghongdianzi.cn

CREATE TABLE users (
来源：http://lr.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jl.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://oo.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://ft.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ea.shxzukj.cn

);
来源：http://fq.newstarts.cn

[Q02] 创建带外键的表
来源：http://lu.gzmigu.cn

CREATE TABLE orders (
来源：http://fj.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xj.jctech888.com.cn

user_id INT NOT NULL,
来源：http://ql.nicolike.cn

amount DECIMAL(10, 2),
来源：http://nj.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tr.asd995.cn

);
来源：http://sl.hahajie.cn

[Q03] 增加列
来源：http://ai.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iq.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://st.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hu.shxzukj.cn

[Q05] 重命名列
来源：http://sk.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sq.huanxung.cn

[Q06] 删除列
来源：http://nn.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bq.huixiangedu.cn

[Q07] 删除表
来源：http://of.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://an.shxzukj.cn

[Q08] 创建普通索引
来源：http://nd.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ja.521024.cn

[Q09] 创建唯一索引
来源：http://qn.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fy.panjiajie.cn

[Q10] 插入单行
来源：http://za.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://do.huixiangedu.cn

[Q11] 一次插入多行
来源：http://hc.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sj.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://ss.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ta.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ap.lnxyls.cn

[Q13] 忽略重复插入
来源：http://ze.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wa.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://av.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rt.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mk.jianghongdianzi.cn

[Q15] 查询全部
来源：http://jx.hnjuh.cn

SELECT * FROM users;
来源：http://ll.panjiajie.cn

[Q16] 查询指定列
来源：http://iy.nszjky.cn

SELECT id, name FROM users;
来源：http://od.yuexingan06.cn

[Q17] 条件查询
来源：http://sx.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bh.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://et.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fp.jianghongdianzi.cn

[Q19] 范围查询
来源：http://gw.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jl.asd995.cn

[Q20] IN 列表
来源：http://yv.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://he.9csxet.cn

[Q21] 空值判断
来源：http://ti.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yw.yuexingan06.cn

[Q22] 排序
来源：http://wl.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://li.szxytkj.cn

[Q23] 分页
来源：http://dw.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zd.yuexingan06.cn

[Q24] 去重
来源：http://ac.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://ll.newstarts.cn

[Q25] 只取前 N 条
来源：http://fb.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nq.colortex.cn

[Q26] 计数
来源：http://pf.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ut.yuexingan06.cn

[Q27] 条件计数
来源：http://cp.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jx.szsharing.cn

[Q28] 求和与平均
来源：http://fg.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nj.szxytkj.cn

[Q29] 最大最小值
来源：http://dk.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vt.jctech888.com.cn

[Q30] 分组统计
来源：http://ic.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://af.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ro.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sc.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://wy.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pn.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://de.huixinmuqiang.cn

[Q33] 多列分组
来源：http://hl.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lj.jctech888.com.cn

[Q34] 每组取第一条
来源：http://uu.chemitech.net.cn

SELECT * FROM (
来源：http://eg.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uj.wgjwhj.cn

) t WHERE rn = 1;
来源：http://bl.shxzukj.cn

[Q35] 内连接
来源：http://hg.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xj.shtwfgs.cn

[Q36] 左连接
来源：http://et.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pw.shxzukj.cn

[Q37] 右连接
来源：http://pq.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mk.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://js.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ui.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://ge.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ta.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dv.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tv.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xr.shtwfgs.cn

[Q41] 多表连接
来源：http://cv.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ky.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://pp.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://du.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://jg.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://jt.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://il.nszjky.cn

[Q43] 标量子查询
来源：http://ba.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zs.colortex.cn

[Q44] IN 子查询
来源：http://vz.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pr.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://kf.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rp.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bp.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qh.hnjuh.cn

[Q47] 与平均值比较
来源：http://we.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://si.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://ex.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yx.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://kr.colortex.cn

[Q49] 更新单行
来源：http://rb.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ff.wgjwhj.cn

[Q50] 批量更新
来源：http://gy.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oo.521024.cn

[Q51] 用子查询更新
来源：http://tq.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pw.bjjhwx.cn

[Q52] 删除指定行
来源：http://nc.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://fn.shtwfgs.cn

[Q53] 按条件删除
来源：http://hq.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pg.huanxung.cn

[Q54] 清空表
来源：http://ac.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://yj.nszjky.cn

[Q55] 排名（并列占位）
来源：http://ai.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cz.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://tm.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bg.jianghongdianzi.cn

[Q57] 行号
来源：http://iy.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jw.9csxet.cn

[Q58] 累计求和
来源：http://xj.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cz.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://rj.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://op.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://jq.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dd.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fw.panjiajie.cn

[Q61] 移动平均
来源：http://uc.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qm.szsharing.cn

[Q62] 分组占比
来源：http://aq.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rp.chemitech.net.cn

[Q63] 开启事务
来源：http://vh.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wj.jianghongdianzi.cn

[Q64] 提交事务
来源：http://su.gzmigu.cn

COMMIT;
来源：http://uc.521024.cn

[Q65] 回滚事务
来源：http://py.panjiajie.cn

ROLLBACK;
来源：http://cm.huixiangedu.cn

[Q66] 行锁查询
来源：http://lq.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xn.bjjhwx.cn


<!-- 参考信息 -->