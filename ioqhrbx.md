代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ox.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tm.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://pm.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://do.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cw.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ug.colortex.cn

[N11] 二叉树中序遍历
来源：http://sg.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gf.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://dv.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uf.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wn.asd995.cn

Java: // 手写递归
来源：http://ez.szsharing.cn

Go:   // 手写递归
来源：http://gi.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fz.szsharing.cn

C#:   // 手写递归
来源：http://si.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wb.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ko.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ts.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wo.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tb.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ab.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yu.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hc.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://de.shxzskj.cn

================================================================================
来源：http://qu.shtwfgs.cn

O. 并发与异步
来源：http://ea.bjjhwx.cn

================================================================================
来源：http://ur.shxzskj.cn

[O01] 启动一个线程
来源：http://aj.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jn.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mv.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://br.colortex.cn

TS:   // 同 JS
来源：http://gb.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://vm.bjjhwx.cn

Go:   go f()
来源：http://kw.nszjky.cn

Ruby: Thread.new { f }
来源：http://cb.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://rp.lnxyls.cn

[O02] 使用线程池
来源：http://zb.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mh.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uj.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://ks.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://mk.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xf.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gc.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qj.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ux.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://zk.szsharing.cn

Py:   with lock: shared += 1
来源：http://so.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://om.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wb.shtwfgs.cn

TS:   // 同 JS
来源：http://mi.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://nx.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xz.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rh.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://lj.hahajie.cn

[O04] 定义异步函数并等待
来源：http://vs.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://jc.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jb.newstarts.cn

JS:   async function f() { await g(); }
来源：http://bw.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xe.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ah.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ci.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ub.colortex.cn

C#:   async Task F() { await G(); }
来源：http://qc.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://vg.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://vp.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oy.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://ln.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://gc.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ur.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ke.9csxet.cn

Ruby: threads.map(&:join)
来源：http://jp.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bf.bjjhwx.cn

[O06] 使用进程池
来源：http://us.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mw.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ri.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://jf.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://bm.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sw.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nf.521024.cn

Ruby: // fork 块
来源：http://gb.huixiangedu.cn

C#:   Parallel.For
来源：http://ep.panjiajie.cn

================================================================================
来源：http://lf.yuntaijiaju.cn

P. 常用工具函数
来源：http://qq.huixinmuqiang.cn

================================================================================
来源：http://pa.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://xd.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://di.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ex.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://vy.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://oo.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://sv.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://qt.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://ok.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://de.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://us.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gv.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rq.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rp.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eo.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bi.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ab.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sx.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xp.521024.cn

[P03] 生成短随机字符串
来源：http://se.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fn.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ji.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fq.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mi.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qr.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nf.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jz.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://if.newstarts.cn

[P04] 求长度
来源：http://hk.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uf.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nu.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ow.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sw.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ia.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://mv.asd995.cn

Ruby: x.length;  x.size
来源：http://nw.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qj.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://uy.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xb.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://en.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gi.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ea.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pm.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qh.9csxet.cn

Ruby: a == b
来源：http://cu.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ek.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tc.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ce.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://wu.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uc.nicolike.cn

TS:   if (x == null) {}
来源：http://ps.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ep.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://yj.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gg.bjjhwx.cn

C#:   if (x is null) {}
来源：http://ve.newstarts.cn

[P07] 防抖与节流
来源：http://yl.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jp.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://rr.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gr.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xi.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wa.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vy.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ns.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://du.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://dy.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xb.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gx.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cc.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ll.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ib.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ya.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mf.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sy.shxzukj.cn

================================================================================
来源：http://wg.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uw.9csxet.cn

================================================================================
来源：http://dp.hahajie.cn

[Q01] 创建表
来源：http://fb.shxzukj.cn

CREATE TABLE users (
来源：http://mp.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rk.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://ai.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://bg.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ny.nicolike.cn

);
来源：http://ca.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://la.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://vo.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jc.chemitech.net.cn

user_id INT NOT NULL,
来源：http://ii.newstarts.cn

amount DECIMAL(10, 2),
来源：http://ak.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gz.nszjky.cn

);
来源：http://et.szxytkj.cn

[Q03] 增加列
来源：http://dt.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kh.bookmarksfly.cn

[Q04] 修改列类型
来源：http://so.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yf.shxzskj.cn

[Q05] 重命名列
来源：http://jc.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.9csxet.cn

[Q06] 删除列
来源：http://qv.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mx.hahajie.cn

[Q07] 删除表
来源：http://np.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://di.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://xt.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xi.huanxung.cn

[Q09] 创建唯一索引
来源：http://kh.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ta.huixiangedu.cn

[Q10] 插入单行
来源：http://bm.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oh.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://ej.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ck.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://lj.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mm.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tl.lnxyls.cn

[Q13] 忽略重复插入
来源：http://gj.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cj.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://gg.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ar.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rq.gzmigu.cn

[Q15] 查询全部
来源：http://nz.huixiangedu.cn

SELECT * FROM users;
来源：http://wd.newstarts.cn

[Q16] 查询指定列
来源：http://jk.shtwfgs.cn

SELECT id, name FROM users;
来源：http://yv.shxzskj.cn

[Q17] 条件查询
来源：http://zc.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sz.wgjwhj.cn

[Q18] 模糊匹配
来源：http://ju.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ol.wgjwhj.cn

[Q19] 范围查询
来源：http://yk.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xy.lnxyls.cn

[Q20] IN 列表
来源：http://tj.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sr.bookmarksfly.cn

[Q21] 空值判断
来源：http://sa.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nk.newstarts.cn

[Q22] 排序
来源：http://xa.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vt.hahajie.cn

[Q23] 分页
来源：http://rs.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eg.shxzukj.cn

[Q24] 去重
来源：http://lx.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ku.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://fl.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xc.colortex.cn

[Q26] 计数
来源：http://ml.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://mr.nicolike.cn

[Q27] 条件计数
来源：http://ww.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ao.521024.cn

[Q28] 求和与平均
来源：http://dn.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zt.chemitech.net.cn

[Q29] 最大最小值
来源：http://pe.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bv.wgjwhj.cn

[Q30] 分组统计
来源：http://et.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jg.shxzskj.cn

[Q31] 分组后过滤
来源：http://pe.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fl.521024.cn

[Q32] 分组拼接字符串
来源：http://mp.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://na.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://im.szxytkj.cn

[Q33] 多列分组
来源：http://hs.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gz.yuexingan06.cn

[Q34] 每组取第一条
来源：http://qv.hahajie.cn

SELECT * FROM (
来源：http://vp.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xm.newstarts.cn

) t WHERE rn = 1;
来源：http://nj.shtwfgs.cn

[Q35] 内连接
来源：http://ti.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wq.panjiajie.cn

[Q36] 左连接
来源：http://ag.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lc.yuexingan06.cn

[Q37] 右连接
来源：http://de.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cc.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mb.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sf.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ry.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://az.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ht.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ya.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cv.muxihuayi.cn

[Q41] 多表连接
来源：http://ks.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yo.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://pu.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://pp.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ko.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://qb.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oh.huanxung.cn

[Q43] 标量子查询
来源：http://uw.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://au.shtwfgs.cn

[Q44] IN 子查询
来源：http://my.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jl.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://rk.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qc.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://se.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sc.yuexingan06.cn

[Q47] 与平均值比较
来源：http://tz.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wo.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://vv.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yr.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://dm.bjjhwx.cn

[Q49] 更新单行
来源：http://oo.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pj.jianghongdianzi.cn

[Q50] 批量更新
来源：http://he.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ot.chemitech.net.cn

[Q51] 用子查询更新
来源：http://kn.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yt.nszjky.cn

[Q52] 删除指定行
来源：http://uv.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://el.bjjhwx.cn

[Q53] 按条件删除
来源：http://hl.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hx.9csxet.cn

[Q54] 清空表
来源：http://bu.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://bl.colortex.cn

[Q55] 排名（并列占位）
来源：http://kw.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ba.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://ra.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bg.chemitech.net.cn

[Q57] 行号
来源：http://ib.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://km.nszjky.cn

[Q58] 累计求和
来源：http://hb.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mp.chemitech.net.cn

[Q59] 分组内累计
来源：http://re.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://td.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://jv.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lg.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gs.szxytkj.cn


<!-- 参考信息 -->