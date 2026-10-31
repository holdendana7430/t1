代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://xb.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ev.nicolike.cn

[N11] 二叉树中序遍历
来源：http://em.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sj.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://st.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fy.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tx.jctech888.com.cn

Java: // 手写递归
来源：http://rn.haigaiapp.cn

Go:   // 手写递归
来源：http://ya.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nq.gzmigu.cn

C#:   // 手写递归
来源：http://mi.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jk.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ms.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bh.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hd.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hn.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yy.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hd.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jm.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://od.huixiangedu.cn

================================================================================
来源：http://vs.hnjuh.cn

O. 并发与异步
来源：http://zs.shtwfgs.cn

================================================================================
来源：http://ao.jctech888.com.cn

[O01] 启动一个线程
来源：http://na.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://px.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jb.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gm.9csxet.cn

TS:   // 同 JS
来源：http://ch.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://za.chemitech.net.cn

Go:   go f()
来源：http://dl.9csxet.cn

Ruby: Thread.new { f }
来源：http://mm.521024.cn

C#:   Task.Run(() => F());
来源：http://uh.haigaiapp.cn

[O02] 使用线程池
来源：http://lh.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uj.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iu.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://al.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://cm.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ry.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nw.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wi.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lg.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://nz.newstarts.cn

Py:   with lock: shared += 1
来源：http://rp.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://md.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ih.bjjhwx.cn

TS:   // 同 JS
来源：http://fq.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://bs.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nq.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iv.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://kp.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://fj.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://lo.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iw.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ip.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qv.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yw.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://um.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ix.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://wm.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://bl.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://gq.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dd.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://gq.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://tu.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aw.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ng.asd995.cn

Ruby: threads.map(&:join)
来源：http://xp.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wy.shxzskj.cn

[O06] 使用进程池
来源：http://kx.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://om.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fw.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://js.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://cm.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mb.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://il.jctech888.com.cn

Ruby: // fork 块
来源：http://ty.szxytkj.cn

C#:   Parallel.For
来源：http://bg.jianghongdianzi.cn

================================================================================
来源：http://oz.nicolike.cn

P. 常用工具函数
来源：http://yy.bjjhwx.cn

================================================================================
来源：http://ak.chemitech.net.cn

[P01] 生成 UUID
来源：http://im.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://lo.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sr.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://hf.9csxet.cn

TS:   crypto.randomUUID()
来源：http://tm.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://dp.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://lz.colortex.cn

Ruby: SecureRandom.uuid
来源：http://oz.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://og.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://nd.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sq.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rj.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bm.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wp.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://og.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pj.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://du.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sm.szxytkj.cn

[P03] 生成短随机字符串
来源：http://lu.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://od.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qu.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xp.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kq.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xg.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ju.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://el.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ju.521024.cn

[P04] 求长度
来源：http://ya.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ds.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lq.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ia.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qh.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://jx.521024.cn

Go:   len(arr);  len(m)
来源：http://cf.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://qq.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://at.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://ac.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cv.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jp.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bq.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://se.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fi.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zc.chemitech.net.cn

Ruby: a == b
来源：http://th.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yg.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zr.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bx.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://lm.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ce.gzmigu.cn

TS:   if (x == null) {}
来源：http://vz.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fi.huanxung.cn

Go:   if x == nil {}
来源：http://yw.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tq.hnjuh.cn

C#:   if (x is null) {}
来源：http://ha.haigaiapp.cn

[P07] 防抖与节流
来源：http://im.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://br.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://gt.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rg.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ue.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://va.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wi.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://es.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lm.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://an.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ib.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dc.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ma.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dr.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://am.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mo.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kf.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ee.colortex.cn

================================================================================
来源：http://sc.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fx.szxytkj.cn

================================================================================
来源：http://oa.newstarts.cn

[Q01] 创建表
来源：http://yu.yuexingan06.cn

CREATE TABLE users (
来源：http://th.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ds.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://ki.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://of.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://at.szsharing.cn

);
来源：http://rx.gzmigu.cn

[Q02] 创建带外键的表
来源：http://tu.newstarts.cn

CREATE TABLE orders (
来源：http://eh.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ys.nicolike.cn

user_id INT NOT NULL,
来源：http://or.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://zd.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qm.chemitech.net.cn

);
来源：http://jx.wgjwhj.cn

[Q03] 增加列
来源：http://kg.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ek.shxzskj.cn

[Q04] 修改列类型
来源：http://vr.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://il.szsharing.cn

[Q05] 重命名列
来源：http://jn.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hp.chemitech.net.cn

[Q06] 删除列
来源：http://ee.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yc.hahajie.cn

[Q07] 删除表
来源：http://nw.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://az.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ga.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aq.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://gy.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qa.9csxet.cn

[Q10] 插入单行
来源：http://au.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ja.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ef.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ha.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://zz.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yi.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eh.nszjky.cn

[Q13] 忽略重复插入
来源：http://zy.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yu.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://bh.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yv.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wn.huanxung.cn

[Q15] 查询全部
来源：http://rf.gzmigu.cn

SELECT * FROM users;
来源：http://fq.newstarts.cn

[Q16] 查询指定列
来源：http://ic.9csxet.cn

SELECT id, name FROM users;
来源：http://cu.jctech888.com.cn

[Q17] 条件查询
来源：http://dw.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mj.panjiajie.cn

[Q18] 模糊匹配
来源：http://ax.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ai.muxihuayi.cn

[Q19] 范围查询
来源：http://ov.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cb.lnxyls.cn

[Q20] IN 列表
来源：http://fh.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ut.shtwfgs.cn

[Q21] 空值判断
来源：http://jp.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hv.hnjuh.cn

[Q22] 排序
来源：http://lm.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ko.nicolike.cn

[Q23] 分页
来源：http://gf.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ym.szxytkj.cn

[Q24] 去重
来源：http://lo.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://xl.nszjky.cn

[Q25] 只取前 N 条
来源：http://dh.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wq.newstarts.cn

[Q26] 计数
来源：http://pn.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://ft.shxzskj.cn

[Q27] 条件计数
来源：http://yu.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bp.9csxet.cn

[Q28] 求和与平均
来源：http://jr.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hv.bookmarksfly.cn

[Q29] 最大最小值
来源：http://dq.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wz.huixiangedu.cn

[Q30] 分组统计
来源：http://xq.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yb.nicolike.cn

[Q31] 分组后过滤
来源：http://mm.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dh.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://qx.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ac.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gv.szsharing.cn

[Q33] 多列分组
来源：http://gz.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vn.muxihuayi.cn

[Q34] 每组取第一条
来源：http://sv.szsharing.cn

SELECT * FROM (
来源：http://jf.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cw.shtwfgs.cn

) t WHERE rn = 1;
来源：http://jc.chemitech.net.cn

[Q35] 内连接
来源：http://za.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://he.bookmarksfly.cn

[Q36] 左连接
来源：http://gu.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kh.huanxung.cn

[Q37] 右连接
来源：http://vn.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vp.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lk.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aq.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://he.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fu.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rz.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oy.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qh.nicolike.cn

[Q41] 多表连接
来源：http://cm.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gl.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://jg.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://db.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://ad.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://eh.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vm.lnxyls.cn

[Q43] 标量子查询
来源：http://au.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bn.yuexingan06.cn

[Q44] IN 子查询
来源：http://si.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sc.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://fz.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tw.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xo.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fa.lnxyls.cn

[Q47] 与平均值比较
来源：http://vm.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xz.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ot.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bo.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://sd.nszjky.cn

[Q49] 更新单行
来源：http://nq.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zy.szxytkj.cn

[Q50] 批量更新
来源：http://fo.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://po.szxytkj.cn

[Q51] 用子查询更新
来源：http://to.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gd.muxihuayi.cn

[Q52] 删除指定行
来源：http://vz.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://or.hahajie.cn

[Q53] 按条件删除
来源：http://bc.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nd.gzmigu.cn

[Q54] 清空表
来源：http://cf.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://ma.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://bf.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dz.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://ex.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kk.haigaiapp.cn

[Q57] 行号
来源：http://tv.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vc.shxzskj.cn

[Q58] 累计求和
来源：http://dk.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://og.nicolike.cn

[Q59] 分组内累计
来源：http://jx.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oe.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://qr.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://te.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ey.huanxung.cn

[Q61] 移动平均
来源：http://jq.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xa.asd995.cn

[Q62] 分组占比
来源：http://ts.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oc.jctech888.com.cn


<!-- 参考信息 -->