代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hv.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hh.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://od.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pm.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://bp.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yo.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mt.shtwfgs.cn

Java: // 手写递归
来源：http://xf.newstarts.cn

Go:   // 手写递归
来源：http://qx.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vh.hnjuh.cn

C#:   // 手写递归
来源：http://db.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vb.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cl.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gz.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xe.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pu.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yf.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pe.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://an.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cb.jianghongdianzi.cn

================================================================================
来源：http://id.huanxung.cn

O. 并发与异步
来源：http://uy.szsharing.cn

================================================================================
来源：http://fd.panjiajie.cn

[O01] 启动一个线程
来源：http://le.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qe.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ha.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kw.yuexingan06.cn

TS:   // 同 JS
来源：http://xf.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://tm.muxihuayi.cn

Go:   go f()
来源：http://we.lnxyls.cn

Ruby: Thread.new { f }
来源：http://gt.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://de.szxytkj.cn

[O02] 使用线程池
来源：http://fq.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xv.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qg.9csxet.cn

JS:   // worker_threads 线程池
来源：http://uo.9csxet.cn

TS:   // worker_threads 线程池
来源：http://jt.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rs.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bw.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yp.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://az.hahajie.cn

[O03] 加锁保护共享数据
来源：http://we.shxzskj.cn

Py:   with lock: shared += 1
来源：http://oz.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://dl.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nm.huixinmuqiang.cn

TS:   // 同 JS
来源：http://yr.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://za.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xr.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jh.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://sl.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://cs.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://eh.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eh.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://tc.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gu.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cf.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hc.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qe.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://sf.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://bi.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://xz.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vy.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://je.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://kn.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jm.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zm.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://nx.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ai.shxzukj.cn

[O06] 使用进程池
来源：http://dd.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sl.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kh.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://hj.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://wl.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nl.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ja.chemitech.net.cn

Ruby: // fork 块
来源：http://cf.panjiajie.cn

C#:   Parallel.For
来源：http://dt.newstarts.cn

================================================================================
来源：http://qz.huixinmuqiang.cn

P. 常用工具函数
来源：http://wh.huanxung.cn

================================================================================
来源：http://tv.huanxung.cn

[P01] 生成 UUID
来源：http://hm.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://yq.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ep.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://dy.nszjky.cn

TS:   crypto.randomUUID()
来源：http://jr.521024.cn

Java: UUID.randomUUID().toString()
来源：http://vv.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://bt.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://mx.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://sz.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://fv.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sc.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://be.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eb.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ys.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pf.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qs.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bq.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eb.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://yr.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sa.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yx.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pr.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uo.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hm.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rv.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wr.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lu.9csxet.cn

[P04] 求长度
来源：http://ta.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nd.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kn.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pe.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://if.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://nj.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://zv.521024.cn

Ruby: x.length;  x.size
来源：http://ch.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pg.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ww.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://px.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zz.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vb.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rv.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mb.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lh.szsharing.cn

Ruby: a == b
来源：http://yk.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ry.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ib.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pk.asd995.cn

PHP:  if (empty($x)) {}
来源：http://vv.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zq.jctech888.com.cn

TS:   if (x == null) {}
来源：http://oi.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lr.newstarts.cn

Go:   if x == nil {}
来源：http://rc.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yz.9csxet.cn

C#:   if (x is null) {}
来源：http://ha.shxzukj.cn

[P07] 防抖与节流
来源：http://ig.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gm.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://je.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yn.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jh.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://we.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kk.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uz.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://za.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://np.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wl.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cp.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nz.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zs.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qi.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xg.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bo.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qg.huixinmuqiang.cn

================================================================================
来源：http://qv.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jt.haigaiapp.cn

================================================================================
来源：http://hv.gzmigu.cn

[Q01] 创建表
来源：http://cw.521024.cn

CREATE TABLE users (
来源：http://eq.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://no.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://mt.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://rc.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cm.newstarts.cn

);
来源：http://ly.newstarts.cn

[Q02] 创建带外键的表
来源：http://im.wgjwhj.cn

CREATE TABLE orders (
来源：http://dq.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mg.9csxet.cn

user_id INT NOT NULL,
来源：http://jd.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://nv.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qw.asd995.cn

);
来源：http://of.bookmarksfly.cn

[Q03] 增加列
来源：http://dr.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hd.wgjwhj.cn

[Q04] 修改列类型
来源：http://vy.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://go.huixiangedu.cn

[Q05] 重命名列
来源：http://qa.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vt.haigaiapp.cn

[Q06] 删除列
来源：http://pj.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ev.hahajie.cn

[Q07] 删除表
来源：http://hp.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://gu.shxzskj.cn

[Q08] 创建普通索引
来源：http://bh.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tq.szxytkj.cn

[Q09] 创建唯一索引
来源：http://ig.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jn.panjiajie.cn

[Q10] 插入单行
来源：http://nx.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yx.chemitech.net.cn

[Q11] 一次插入多行
来源：http://cd.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qn.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://is.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sp.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ab.shxzukj.cn

[Q13] 忽略重复插入
来源：http://ie.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tm.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://ph.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ns.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ws.nicolike.cn

[Q15] 查询全部
来源：http://lh.haigaiapp.cn

SELECT * FROM users;
来源：http://vf.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://aa.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://ng.wgjwhj.cn

[Q17] 条件查询
来源：http://ez.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ny.shtwfgs.cn

[Q18] 模糊匹配
来源：http://xd.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://be.szsharing.cn

[Q19] 范围查询
来源：http://hs.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cd.bookmarksfly.cn

[Q20] IN 列表
来源：http://me.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rl.yuntaijiaju.cn

[Q21] 空值判断
来源：http://tn.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wn.gzmigu.cn

[Q22] 排序
来源：http://of.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qg.521024.cn

[Q23] 分页
来源：http://hb.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ks.jctech888.com.cn

[Q24] 去重
来源：http://dg.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://fd.szsharing.cn

[Q25] 只取前 N 条
来源：http://vi.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gu.yuntaijiaju.cn

[Q26] 计数
来源：http://at.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://wh.9csxet.cn

[Q27] 条件计数
来源：http://bf.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xt.szxytkj.cn

[Q28] 求和与平均
来源：http://oe.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pn.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://oz.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lt.jctech888.com.cn

[Q30] 分组统计
来源：http://hj.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bu.szsharing.cn

[Q31] 分组后过滤
来源：http://lh.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://of.nszjky.cn

[Q32] 分组拼接字符串
来源：http://qf.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uv.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://da.nicolike.cn

[Q33] 多列分组
来源：http://dz.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jy.colortex.cn

[Q34] 每组取第一条
来源：http://hx.nicolike.cn

SELECT * FROM (
来源：http://pu.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tw.colortex.cn

) t WHERE rn = 1;
来源：http://vj.nszjky.cn

[Q35] 内连接
来源：http://sd.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jv.jctech888.com.cn

[Q36] 左连接
来源：http://it.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ze.hahajie.cn

[Q37] 右连接
来源：http://cw.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ts.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rh.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qf.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://dq.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uh.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wa.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qn.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zw.lnxyls.cn

[Q41] 多表连接
来源：http://wp.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tl.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://gq.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://wq.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://ls.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://rc.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cp.9csxet.cn

[Q43] 标量子查询
来源：http://fo.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yc.huixiangedu.cn

[Q44] IN 子查询
来源：http://bk.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ad.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://kt.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rw.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://to.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ss.chemitech.net.cn

[Q47] 与平均值比较
来源：http://yr.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qk.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://on.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kj.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://dw.szxytkj.cn

[Q49] 更新单行
来源：http://tp.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nk.bjjhwx.cn

[Q50] 批量更新
来源：http://zd.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ts.colortex.cn

[Q51] 用子查询更新
来源：http://ga.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vg.shtwfgs.cn

[Q52] 删除指定行
来源：http://gk.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://yu.szsharing.cn

[Q53] 按条件删除
来源：http://lx.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://du.muxihuayi.cn

[Q54] 清空表
来源：http://hk.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://ml.hahajie.cn

[Q55] 排名（并列占位）
来源：http://mb.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ae.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://tp.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uj.nicolike.cn

[Q57] 行号
来源：http://ks.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mh.nicolike.cn

[Q58] 累计求和
来源：http://da.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ph.9csxet.cn

[Q59] 分组内累计
来源：http://cv.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gl.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://es.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hj.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dt.newstarts.cn

[Q61] 移动平均
来源：http://ir.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gx.colortex.cn

[Q62] 分组占比
来源：http://eu.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lu.hnjuh.cn


<!-- 参考信息 -->