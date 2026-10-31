代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://kd.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kl.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://pc.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vd.521024.cn

PHP:  // 手写递归函数
来源：http://lg.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vr.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lq.yuntaijiaju.cn

Java: // 手写递归
来源：http://ve.szxytkj.cn

Go:   // 手写递归
来源：http://kq.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pj.szsharing.cn

C#:   // 手写递归
来源：http://wm.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ad.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://em.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fj.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ro.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yw.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ov.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://by.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kg.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mx.yuntaijiaju.cn

================================================================================
来源：http://vt.yuexingan06.cn

O. 并发与异步
来源：http://hp.huixinmuqiang.cn

================================================================================
来源：http://sj.shtwfgs.cn

[O01] 启动一个线程
来源：http://im.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jo.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hb.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zl.shxzukj.cn

TS:   // 同 JS
来源：http://zk.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://nq.hahajie.cn

Go:   go f()
来源：http://yt.hahajie.cn

Ruby: Thread.new { f }
来源：http://yk.521024.cn

C#:   Task.Run(() => F());
来源：http://ts.muxihuayi.cn

[O02] 使用线程池
来源：http://ak.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sp.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wq.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://hv.asd995.cn

TS:   // worker_threads 线程池
来源：http://nr.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wn.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dm.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ri.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ao.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://un.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://jt.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://nz.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kj.jctech888.com.cn

TS:   // 同 JS
来源：http://vw.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://et.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tg.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://df.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://uv.huanxung.cn

[O04] 定义异步函数并等待
来源：http://gy.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://vv.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aq.hahajie.cn

JS:   async function f() { await g(); }
来源：http://pk.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ux.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://er.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lx.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bn.521024.cn

C#:   async Task F() { await G(); }
来源：http://st.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://fb.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://fb.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gq.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://wg.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://rr.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zb.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kc.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://co.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ym.shxzskj.cn

[O06] 使用进程池
来源：http://oy.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hu.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fb.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://rn.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://wb.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://va.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wa.haigaiapp.cn

Ruby: // fork 块
来源：http://xz.nicolike.cn

C#:   Parallel.For
来源：http://yh.huixiangedu.cn

================================================================================
来源：http://rm.haigaiapp.cn

P. 常用工具函数
来源：http://vu.colortex.cn

================================================================================
来源：http://il.huixiangedu.cn

[P01] 生成 UUID
来源：http://fj.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ke.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lf.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://hq.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://pu.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://xp.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://uh.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://ji.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://md.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://ny.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tu.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mn.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cc.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wi.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ek.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pq.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sf.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cb.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://sf.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uv.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nr.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kw.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oy.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wm.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dp.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ob.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ps.gzmigu.cn

[P04] 求长度
来源：http://fe.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nc.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wu.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bg.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nq.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://xf.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ws.521024.cn

Ruby: x.length;  x.size
来源：http://qj.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rv.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://nf.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zd.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oh.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://um.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kd.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kk.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fq.shtwfgs.cn

Ruby: a == b
来源：http://bt.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dl.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ef.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sm.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://rc.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pt.panjiajie.cn

TS:   if (x == null) {}
来源：http://gb.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yf.lnxyls.cn

Go:   if x == nil {}
来源：http://cy.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ah.shxzukj.cn

C#:   if (x is null) {}
来源：http://xm.hnjuh.cn

[P07] 防抖与节流
来源：http://pt.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cv.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://pp.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iu.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oy.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ug.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uv.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sp.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vm.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://mx.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dt.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sc.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gs.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ih.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wc.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rq.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kx.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://do.9csxet.cn

================================================================================
来源：http://kt.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fk.panjiajie.cn

================================================================================
来源：http://fn.huixinmuqiang.cn

[Q01] 创建表
来源：http://co.gzmigu.cn

CREATE TABLE users (
来源：http://sj.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rk.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ys.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://wy.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qj.huixiangedu.cn

);
来源：http://kq.newstarts.cn

[Q02] 创建带外键的表
来源：http://yj.chemitech.net.cn

CREATE TABLE orders (
来源：http://ug.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tf.hahajie.cn

user_id INT NOT NULL,
来源：http://kv.newstarts.cn

amount DECIMAL(10, 2),
来源：http://dt.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ey.huixinmuqiang.cn

);
来源：http://rj.panjiajie.cn

[Q03] 增加列
来源：http://fx.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dg.nszjky.cn

[Q04] 修改列类型
来源：http://kg.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gl.jctech888.com.cn

[Q05] 重命名列
来源：http://pz.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gd.521024.cn

[Q06] 删除列
来源：http://nm.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rc.muxihuayi.cn

[Q07] 删除表
来源：http://qr.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://ki.shxzukj.cn

[Q08] 创建普通索引
来源：http://oa.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mf.hnjuh.cn

[Q09] 创建唯一索引
来源：http://pb.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ov.wgjwhj.cn

[Q10] 插入单行
来源：http://yi.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hc.huanxung.cn

[Q11] 一次插入多行
来源：http://tg.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yg.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://ts.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://al.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kr.nicolike.cn

[Q13] 忽略重复插入
来源：http://qr.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ey.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://as.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ix.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fx.gzmigu.cn

[Q15] 查询全部
来源：http://up.chemitech.net.cn

SELECT * FROM users;
来源：http://et.huanxung.cn

[Q16] 查询指定列
来源：http://sv.bjjhwx.cn

SELECT id, name FROM users;
来源：http://nd.colortex.cn

[Q17] 条件查询
来源：http://ke.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ph.haigaiapp.cn

[Q18] 模糊匹配
来源：http://md.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mn.9csxet.cn

[Q19] 范围查询
来源：http://pu.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jj.muxihuayi.cn

[Q20] IN 列表
来源：http://kk.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pv.shxzskj.cn

[Q21] 空值判断
来源：http://pi.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tx.hnjuh.cn

[Q22] 排序
来源：http://ka.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://by.yuexingan06.cn

[Q23] 分页
来源：http://qr.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xo.szsharing.cn

[Q24] 去重
来源：http://fc.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://lx.9csxet.cn

[Q25] 只取前 N 条
来源：http://gx.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fv.panjiajie.cn

[Q26] 计数
来源：http://fv.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://su.wgjwhj.cn

[Q27] 条件计数
来源：http://lc.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mw.haigaiapp.cn

[Q28] 求和与平均
来源：http://yw.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xz.huanxung.cn

[Q29] 最大最小值
来源：http://jl.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ac.shxzskj.cn

[Q30] 分组统计
来源：http://fu.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jn.gzmigu.cn

[Q31] 分组后过滤
来源：http://ah.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rf.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://nt.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vq.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://au.haigaiapp.cn

[Q33] 多列分组
来源：http://ey.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xg.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://af.bookmarksfly.cn

SELECT * FROM (
来源：http://rg.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ap.newstarts.cn

) t WHERE rn = 1;
来源：http://uu.shxzskj.cn

[Q35] 内连接
来源：http://yt.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kb.hahajie.cn

[Q36] 左连接
来源：http://az.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wo.yuexingan06.cn

[Q37] 右连接
来源：http://le.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ck.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ny.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jg.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://lg.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ft.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sg.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qh.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ha.szsharing.cn

[Q41] 多表连接
来源：http://gs.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fu.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ji.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://jk.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://ju.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://li.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sl.bookmarksfly.cn

[Q43] 标量子查询
来源：http://yo.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bk.colortex.cn

[Q44] IN 子查询
来源：http://am.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wn.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://dn.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tx.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nc.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qu.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://km.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ot.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://ep.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fm.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://jz.huixiangedu.cn

[Q49] 更新单行
来源：http://ps.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gf.colortex.cn

[Q50] 批量更新
来源：http://tk.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qw.yuexingan06.cn

[Q51] 用子查询更新
来源：http://wl.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xh.wgjwhj.cn

[Q52] 删除指定行
来源：http://ny.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ps.huixiangedu.cn

[Q53] 按条件删除
来源：http://mn.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fm.nicolike.cn

[Q54] 清空表
来源：http://ce.521024.cn

TRUNCATE TABLE logs;
来源：http://xk.newstarts.cn

[Q55] 排名（并列占位）
来源：http://dq.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gh.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://cx.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ki.bookmarksfly.cn

[Q57] 行号
来源：http://nd.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oq.huixiangedu.cn

[Q58] 累计求和
来源：http://wf.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eh.szsharing.cn

[Q59] 分组内累计
来源：http://zk.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zx.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://yx.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kz.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pq.shxzukj.cn

[Q61] 移动平均
来源：http://vf.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xo.gzmigu.cn

[Q62] 分组占比
来源：http://ae.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kv.jianghongdianzi.cn


<!-- 参考信息 -->