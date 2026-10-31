代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wv.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ja.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://ml.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mq.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ud.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vh.9csxet.cn

[N11] 二叉树中序遍历
来源：http://yu.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tv.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://cc.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nn.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hr.yuexingan06.cn

Java: // 手写递归
来源：http://se.hahajie.cn

Go:   // 手写递归
来源：http://yd.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bd.yuntaijiaju.cn

C#:   // 手写递归
来源：http://du.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ef.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wl.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rb.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lg.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ac.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ig.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yk.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pn.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ah.szsharing.cn

================================================================================
来源：http://nb.szsharing.cn

O. 并发与异步
来源：http://vq.jianghongdianzi.cn

================================================================================
来源：http://pe.yuexingan06.cn

[O01] 启动一个线程
来源：http://xm.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zf.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sw.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ba.bookmarksfly.cn

TS:   // 同 JS
来源：http://rw.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://yj.shtwfgs.cn

Go:   go f()
来源：http://gc.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://jd.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://hz.huixiangedu.cn

[O02] 使用线程池
来源：http://jw.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cj.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ry.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://hq.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://dx.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tw.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nt.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://br.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://md.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://xx.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://er.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://wc.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fo.hnjuh.cn

TS:   // 同 JS
来源：http://uw.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://gg.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cq.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://un.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://xb.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://to.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://mi.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xa.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://xe.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vh.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://za.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ih.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ln.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://eq.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://bg.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://zb.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tr.asd995.cn

JS:   await Promise.all(tasks)
来源：http://sm.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://xn.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lh.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fg.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://tl.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qu.asd995.cn

[O06] 使用进程池
来源：http://xr.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tg.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rk.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://qc.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://eh.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bk.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eu.nszjky.cn

Ruby: // fork 块
来源：http://cn.shxzukj.cn

C#:   Parallel.For
来源：http://iu.yuexingan06.cn

================================================================================
来源：http://ke.jianghongdianzi.cn

P. 常用工具函数
来源：http://bo.shtwfgs.cn

================================================================================
来源：http://fk.hahajie.cn

[P01] 生成 UUID
来源：http://rj.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://dr.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ax.hahajie.cn

JS:   crypto.randomUUID()
来源：http://ht.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://jv.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://ao.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://ix.asd995.cn

Ruby: SecureRandom.uuid
来源：http://ca.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://uh.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://sa.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ub.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mc.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lu.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://an.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://da.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vs.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kq.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qc.huanxung.cn

[P03] 生成短随机字符串
来源：http://tl.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vw.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vl.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rh.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mo.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vq.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sc.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qr.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nu.colortex.cn

[P04] 求长度
来源：http://cx.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rz.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gr.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://as.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pc.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://fd.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://kj.lnxyls.cn

Ruby: x.length;  x.size
来源：http://no.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://of.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://iw.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://br.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sx.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://id.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vw.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sm.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kl.shtwfgs.cn

Ruby: a == b
来源：http://rl.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sa.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sb.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ci.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://oo.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tm.colortex.cn

TS:   if (x == null) {}
来源：http://qu.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sg.hahajie.cn

Go:   if x == nil {}
来源：http://su.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mx.shxzskj.cn

C#:   if (x is null) {}
来源：http://aj.shtwfgs.cn

[P07] 防抖与节流
来源：http://is.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ew.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://jk.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://no.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ek.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wd.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ow.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://we.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hw.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ry.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mn.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qm.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eo.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qz.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gx.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eq.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dj.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ek.hahajie.cn

================================================================================
来源：http://ec.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gk.yuexingan06.cn

================================================================================
来源：http://dp.szsharing.cn

[Q01] 创建表
来源：http://hn.jctech888.com.cn

CREATE TABLE users (
来源：http://kz.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lw.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://df.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://nv.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jw.bjjhwx.cn

);
来源：http://jd.szsharing.cn

[Q02] 创建带外键的表
来源：http://ql.shxzukj.cn

CREATE TABLE orders (
来源：http://qj.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bg.shtwfgs.cn

user_id INT NOT NULL,
来源：http://pa.hahajie.cn

amount DECIMAL(10, 2),
来源：http://vh.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bp.wgjwhj.cn

);
来源：http://xo.shxzukj.cn

[Q03] 增加列
来源：http://iv.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://of.chemitech.net.cn

[Q04] 修改列类型
来源：http://ct.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://px.muxihuayi.cn

[Q05] 重命名列
来源：http://kg.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qy.asd995.cn

[Q06] 删除列
来源：http://rl.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://km.521024.cn

[Q07] 删除表
来源：http://uw.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://wk.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://vr.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://um.shxzskj.cn

[Q09] 创建唯一索引
来源：http://tq.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bw.shxzukj.cn

[Q10] 插入单行
来源：http://lx.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nb.nszjky.cn

[Q11] 一次插入多行
来源：http://gl.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fw.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://nv.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ox.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ra.gzmigu.cn

[Q13] 忽略重复插入
来源：http://fn.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xu.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://xk.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gw.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bd.colortex.cn

[Q15] 查询全部
来源：http://pw.bjjhwx.cn

SELECT * FROM users;
来源：http://rq.panjiajie.cn

[Q16] 查询指定列
来源：http://im.yuexingan06.cn

SELECT id, name FROM users;
来源：http://hr.asd995.cn

[Q17] 条件查询
来源：http://pd.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mm.nszjky.cn

[Q18] 模糊匹配
来源：http://zb.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ml.newstarts.cn

[Q19] 范围查询
来源：http://tq.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ep.nszjky.cn

[Q20] IN 列表
来源：http://kk.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ny.nicolike.cn

[Q21] 空值判断
来源：http://sg.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qd.jctech888.com.cn

[Q22] 排序
来源：http://tf.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://db.jctech888.com.cn

[Q23] 分页
来源：http://ao.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eb.chemitech.net.cn

[Q24] 去重
来源：http://xm.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ye.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://lj.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pk.gzmigu.cn

[Q26] 计数
来源：http://wh.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://kv.szsharing.cn

[Q27] 条件计数
来源：http://yl.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hb.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://yj.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wv.nicolike.cn

[Q29] 最大最小值
来源：http://ba.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://su.szxytkj.cn

[Q30] 分组统计
来源：http://le.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xo.nszjky.cn

[Q31] 分组后过滤
来源：http://ss.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xs.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://db.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://il.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gp.yuntaijiaju.cn

[Q33] 多列分组
来源：http://it.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rn.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://ua.shxzukj.cn

SELECT * FROM (
来源：http://sl.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qm.newstarts.cn

) t WHERE rn = 1;
来源：http://ya.hnjuh.cn

[Q35] 内连接
来源：http://wh.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ce.bookmarksfly.cn

[Q36] 左连接
来源：http://hs.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yn.newstarts.cn

[Q37] 右连接
来源：http://pw.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ch.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ex.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xl.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://ak.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://co.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jq.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://de.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uw.jctech888.com.cn

[Q41] 多表连接
来源：http://vm.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ni.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://yc.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://le.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://bv.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://yu.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yg.newstarts.cn

[Q43] 标量子查询
来源：http://iw.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hy.colortex.cn

[Q44] IN 子查询
来源：http://rc.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xr.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://ta.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zs.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qh.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ml.shxzskj.cn

[Q47] 与平均值比较
来源：http://dp.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xy.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://se.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://of.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://ib.nicolike.cn

[Q49] 更新单行
来源：http://rn.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ac.muxihuayi.cn

[Q50] 批量更新
来源：http://sk.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jm.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://ra.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wk.shxzukj.cn

[Q52] 删除指定行
来源：http://qu.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://ya.huanxung.cn

[Q53] 按条件删除
来源：http://ab.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fn.chemitech.net.cn

[Q54] 清空表
来源：http://wk.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://kt.asd995.cn

[Q55] 排名（并列占位）
来源：http://ad.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://li.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://sy.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://of.muxihuayi.cn

[Q57] 行号
来源：http://qh.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://si.muxihuayi.cn

[Q58] 累计求和
来源：http://qf.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tr.panjiajie.cn

[Q59] 分组内累计
来源：http://gc.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kk.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://xb.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vx.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bi.huanxung.cn


<!-- 参考信息 -->