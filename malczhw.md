代发 wailian999

PHP:  // 手写递归函数
来源：http://ch.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ab.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qo.nicolike.cn

Java: // 手写递归
来源：http://zv.panjiajie.cn

Go:   // 手写递归
来源：http://iq.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ng.hahajie.cn

C#:   // 手写递归
来源：http://dk.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wd.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ch.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vr.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gt.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ct.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bj.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://go.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qu.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ce.bookmarksfly.cn

================================================================================
来源：http://vt.bjjhwx.cn

O. 并发与异步
来源：http://zj.521024.cn

================================================================================
来源：http://sl.nicolike.cn

[O01] 启动一个线程
来源：http://ic.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ki.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cu.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rn.wgjwhj.cn

TS:   // 同 JS
来源：http://np.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://de.huixinmuqiang.cn

Go:   go f()
来源：http://qh.hnjuh.cn

Ruby: Thread.new { f }
来源：http://qr.521024.cn

C#:   Task.Run(() => F());
来源：http://js.huanxung.cn

[O02] 使用线程池
来源：http://wf.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pu.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oi.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://qn.nicolike.cn

TS:   // worker_threads 线程池
来源：http://he.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dg.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vj.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ki.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pw.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://jk.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://wg.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://jf.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://js.asd995.cn

TS:   // 同 JS
来源：http://zm.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://rm.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://et.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jv.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://yy.newstarts.cn

[O04] 定义异步函数并等待
来源：http://ks.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://qh.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dt.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://gz.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cv.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ot.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ip.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ey.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://nx.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://uh.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://dz.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sc.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://xq.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://dx.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ua.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qq.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://xh.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://my.chemitech.net.cn

[O06] 使用进程池
来源：http://mp.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vy.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://es.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://wa.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://gg.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dj.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dw.521024.cn

Ruby: // fork 块
来源：http://kz.huanxung.cn

C#:   Parallel.For
来源：http://rl.newstarts.cn

================================================================================
来源：http://qw.huixinmuqiang.cn

P. 常用工具函数
来源：http://iy.huixinmuqiang.cn

================================================================================
来源：http://cu.gzmigu.cn

[P01] 生成 UUID
来源：http://ru.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://vh.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kk.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://jy.jctech888.com.cn

TS:   crypto.randomUUID()
来源：http://bt.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://mh.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://fe.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://ek.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://ow.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://hu.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bs.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://th.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gm.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oy.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kf.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dp.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dn.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sa.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://jk.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oj.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yy.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yj.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hx.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yu.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://so.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zk.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pv.newstarts.cn

[P04] 求长度
来源：http://fu.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pz.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zk.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://et.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://un.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://ws.nszjky.cn

Go:   len(arr);  len(m)
来源：http://oi.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://iz.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://aq.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://yq.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xe.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zt.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lx.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wk.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hj.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ae.szxytkj.cn

Ruby: a == b
来源：http://nl.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eh.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tr.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lx.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://df.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nq.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://hn.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sg.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://oi.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fq.huixiangedu.cn

C#:   if (x is null) {}
来源：http://ks.haigaiapp.cn

[P07] 防抖与节流
来源：http://aw.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kv.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://to.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gv.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kl.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fo.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lk.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nz.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bg.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://iw.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wp.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cs.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yf.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fk.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://is.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lf.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://la.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fh.nicolike.cn

================================================================================
来源：http://as.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bl.muxihuayi.cn

================================================================================
来源：http://sc.shtwfgs.cn

[Q01] 创建表
来源：http://pk.jianghongdianzi.cn

CREATE TABLE users (
来源：http://yh.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sn.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://pk.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://dm.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lj.shtwfgs.cn

);
来源：http://nv.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://my.bookmarksfly.cn

CREATE TABLE orders (
来源：http://uk.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bu.huixiangedu.cn

user_id INT NOT NULL,
来源：http://cu.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://pm.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ud.haigaiapp.cn

);
来源：http://rl.jianghongdianzi.cn

[Q03] 增加列
来源：http://zh.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ji.gzmigu.cn

[Q04] 修改列类型
来源：http://yk.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hx.nicolike.cn

[Q05] 重命名列
来源：http://ep.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rm.shxzskj.cn

[Q06] 删除列
来源：http://uu.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ca.huanxung.cn

[Q07] 删除表
来源：http://zm.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://ui.9csxet.cn

[Q08] 创建普通索引
来源：http://ly.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://im.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://ty.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zk.haigaiapp.cn

[Q10] 插入单行
来源：http://yw.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ux.yuexingan06.cn

[Q11] 一次插入多行
来源：http://hv.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rz.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://bk.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bn.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xr.szxytkj.cn

[Q13] 忽略重复插入
来源：http://jg.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xq.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://px.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vh.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wn.jctech888.com.cn

[Q15] 查询全部
来源：http://lb.shxzskj.cn

SELECT * FROM users;
来源：http://rt.huanxung.cn

[Q16] 查询指定列
来源：http://so.nicolike.cn

SELECT id, name FROM users;
来源：http://sz.jianghongdianzi.cn

[Q17] 条件查询
来源：http://ks.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hb.hnjuh.cn

[Q18] 模糊匹配
来源：http://bp.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hj.panjiajie.cn

[Q19] 范围查询
来源：http://zc.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sm.shxzukj.cn

[Q20] IN 列表
来源：http://pl.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ii.9csxet.cn

[Q21] 空值判断
来源：http://uo.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bz.asd995.cn

[Q22] 排序
来源：http://eo.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lq.szsharing.cn

[Q23] 分页
来源：http://qt.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rg.nszjky.cn

[Q24] 去重
来源：http://dw.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://kz.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://ia.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ep.nszjky.cn

[Q26] 计数
来源：http://gp.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://uf.shxzukj.cn

[Q27] 条件计数
来源：http://ef.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xv.huanxung.cn

[Q28] 求和与平均
来源：http://mp.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lx.szsharing.cn

[Q29] 最大最小值
来源：http://ok.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ji.colortex.cn

[Q30] 分组统计
来源：http://kw.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xz.shxzskj.cn

[Q31] 分组后过滤
来源：http://ah.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://je.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ll.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eu.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xa.jctech888.com.cn

[Q33] 多列分组
来源：http://js.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qc.lnxyls.cn

[Q34] 每组取第一条
来源：http://gi.huixiangedu.cn

SELECT * FROM (
来源：http://bi.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vi.szxytkj.cn

) t WHERE rn = 1;
来源：http://oa.newstarts.cn

[Q35] 内连接
来源：http://xa.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ec.jianghongdianzi.cn

[Q36] 左连接
来源：http://pp.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ci.bookmarksfly.cn

[Q37] 右连接
来源：http://wi.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kr.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ry.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dx.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://uw.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fo.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tf.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xu.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nf.shtwfgs.cn

[Q41] 多表连接
来源：http://gz.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lj.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://zo.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://cg.521024.cn

[Q42] 连接条件附加过滤
来源：http://hw.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://ru.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gb.bookmarksfly.cn

[Q43] 标量子查询
来源：http://qb.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yz.shtwfgs.cn

[Q44] IN 子查询
来源：http://tk.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fd.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://kd.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lz.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sx.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ja.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://lk.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fz.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://tr.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pu.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://rg.hahajie.cn

[Q49] 更新单行
来源：http://qk.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kd.huixiangedu.cn

[Q50] 批量更新
来源：http://kr.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cm.bjjhwx.cn

[Q51] 用子查询更新
来源：http://lp.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mx.jctech888.com.cn

[Q52] 删除指定行
来源：http://mu.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://wx.shtwfgs.cn

[Q53] 按条件删除
来源：http://fl.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kf.shxzukj.cn

[Q54] 清空表
来源：http://il.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ab.szsharing.cn

[Q55] 排名（并列占位）
来源：http://uu.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tb.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://lp.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qe.yuexingan06.cn

[Q57] 行号
来源：http://lz.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://na.chemitech.net.cn

[Q58] 累计求和
来源：http://ex.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vv.hahajie.cn

[Q59] 分组内累计
来源：http://zc.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ni.521024.cn

[Q60] 取上一行 / 下一行
来源：http://ep.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dq.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ku.9csxet.cn

[Q61] 移动平均
来源：http://bf.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ww.bjjhwx.cn

[Q62] 分组占比
来源：http://ef.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eo.panjiajie.cn

[Q63] 开启事务
来源：http://oh.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://in.yuexingan06.cn

[Q64] 提交事务
来源：http://uu.yuntaijiaju.cn

COMMIT;
来源：http://en.nszjky.cn


<!-- 参考信息 -->