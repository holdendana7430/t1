代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://il.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eu.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://kw.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zz.newstarts.cn

PHP:  // 手写递归函数
来源：http://ej.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qa.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iq.newstarts.cn

Java: // 手写递归
来源：http://qk.9csxet.cn

Go:   // 手写递归
来源：http://qj.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pf.lnxyls.cn

C#:   // 手写递归
来源：http://ba.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ws.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vj.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ex.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ph.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iw.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fp.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ih.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qh.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sm.haigaiapp.cn

================================================================================
来源：http://tk.gzmigu.cn

O. 并发与异步
来源：http://ti.lnxyls.cn

================================================================================
来源：http://et.bookmarksfly.cn

[O01] 启动一个线程
来源：http://kf.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cl.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gb.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://er.shxzskj.cn

TS:   // 同 JS
来源：http://yy.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://yr.jctech888.com.cn

Go:   go f()
来源：http://zo.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://xp.9csxet.cn

C#:   Task.Run(() => F());
来源：http://zj.huanxung.cn

[O02] 使用线程池
来源：http://ih.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kz.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vu.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://ep.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://kc.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qk.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://un.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vq.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://go.521024.cn

[O03] 加锁保护共享数据
来源：http://aj.shxzukj.cn

Py:   with lock: shared += 1
来源：http://qi.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://vh.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fc.jianghongdianzi.cn

TS:   // 同 JS
来源：http://xx.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://oa.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lw.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rs.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://kr.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://vd.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://nw.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fz.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://qp.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ah.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://si.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://en.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xf.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://tc.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://rg.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://to.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lo.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://ju.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://ao.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zi.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://as.asd995.cn

Ruby: threads.map(&:join)
来源：http://lr.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wy.521024.cn

[O06] 使用进程池
来源：http://dl.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mt.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ll.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://da.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ig.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ao.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ep.jianghongdianzi.cn

Ruby: // fork 块
来源：http://qn.9csxet.cn

C#:   Parallel.For
来源：http://bb.521024.cn

================================================================================
来源：http://bo.nicolike.cn

P. 常用工具函数
来源：http://zu.shtwfgs.cn

================================================================================
来源：http://dr.lnxyls.cn

[P01] 生成 UUID
来源：http://so.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://ue.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vh.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://nd.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://fg.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://lw.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://ok.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://tb.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://ba.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://na.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://on.jianghongdianzi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hd.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hb.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://id.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lx.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ea.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ff.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qb.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://ie.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hd.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wz.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mi.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://af.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nb.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fg.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xc.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ku.gzmigu.cn

[P04] 求长度
来源：http://bo.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cs.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tx.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sn.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xp.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://fy.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://my.panjiajie.cn

Ruby: x.length;  x.size
来源：http://wu.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://el.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://xg.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dm.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wk.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ue.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fj.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bf.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fz.gzmigu.cn

Ruby: a == b
来源：http://gv.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jg.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pt.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ge.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://eq.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dp.nszjky.cn

TS:   if (x == null) {}
来源：http://wt.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kd.nszjky.cn

Go:   if x == nil {}
来源：http://jy.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ze.bjjhwx.cn

C#:   if (x is null) {}
来源：http://dx.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://uu.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ck.521024.cn

PHP:  // 手写时间戳比较
来源：http://ja.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pk.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uy.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ms.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vj.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cl.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nu.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://ov.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qb.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sw.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fq.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eq.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gb.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://df.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tk.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sg.huixinmuqiang.cn

================================================================================
来源：http://dl.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mg.wgjwhj.cn

================================================================================
来源：http://vs.colortex.cn

[Q01] 创建表
来源：http://il.colortex.cn

CREATE TABLE users (
来源：http://pv.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lm.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://xu.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://js.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ey.asd995.cn

);
来源：http://qo.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://nl.yuexingan06.cn

CREATE TABLE orders (
来源：http://sy.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lf.hahajie.cn

user_id INT NOT NULL,
来源：http://pv.szsharing.cn

amount DECIMAL(10, 2),
来源：http://qh.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vb.521024.cn

);
来源：http://hp.szxytkj.cn

[Q03] 增加列
来源：http://dw.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ii.szsharing.cn

[Q04] 修改列类型
来源：http://iu.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ye.huanxung.cn

[Q05] 重命名列
来源：http://rr.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gq.521024.cn

[Q06] 删除列
来源：http://sk.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ku.wgjwhj.cn

[Q07] 删除表
来源：http://to.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://uo.panjiajie.cn

[Q08] 创建普通索引
来源：http://rt.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ye.szxytkj.cn

[Q09] 创建唯一索引
来源：http://yz.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ff.bookmarksfly.cn

[Q10] 插入单行
来源：http://wr.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ep.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://jt.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qi.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://nf.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ew.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sn.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://jm.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mr.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://mw.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jz.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fh.muxihuayi.cn

[Q15] 查询全部
来源：http://aj.hahajie.cn

SELECT * FROM users;
来源：http://jd.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://hm.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://fc.colortex.cn

[Q17] 条件查询
来源：http://qe.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bc.nszjky.cn

[Q18] 模糊匹配
来源：http://rv.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yn.jctech888.com.cn

[Q19] 范围查询
来源：http://qz.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yb.panjiajie.cn

[Q20] IN 列表
来源：http://pj.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ij.shxzskj.cn

[Q21] 空值判断
来源：http://zn.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://py.muxihuayi.cn

[Q22] 排序
来源：http://am.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zt.szsharing.cn

[Q23] 分页
来源：http://fn.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://et.nicolike.cn

[Q24] 去重
来源：http://qn.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://sb.nszjky.cn

[Q25] 只取前 N 条
来源：http://ti.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fl.colortex.cn

[Q26] 计数
来源：http://zi.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://lp.szsharing.cn

[Q27] 条件计数
来源：http://rk.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rt.521024.cn

[Q28] 求和与平均
来源：http://bq.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ry.wgjwhj.cn

[Q29] 最大最小值
来源：http://nv.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ls.521024.cn

[Q30] 分组统计
来源：http://bk.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hl.shxzukj.cn

[Q31] 分组后过滤
来源：http://fo.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mh.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://ql.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://if.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bj.haigaiapp.cn

[Q33] 多列分组
来源：http://tp.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bl.chemitech.net.cn

[Q34] 每组取第一条
来源：http://tf.hahajie.cn

SELECT * FROM (
来源：http://pn.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ig.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://eh.huixinmuqiang.cn

[Q35] 内连接
来源：http://jp.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qp.yuexingan06.cn

[Q36] 左连接
来源：http://ep.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vi.gzmigu.cn

[Q37] 右连接
来源：http://rh.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hl.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nk.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ro.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ur.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cr.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://by.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kd.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kb.shxzukj.cn

[Q41] 多表连接
来源：http://jh.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jb.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://tg.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://bp.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://sm.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://gx.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oo.nszjky.cn

[Q43] 标量子查询
来源：http://xk.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dz.lnxyls.cn

[Q44] IN 子查询
来源：http://nn.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hc.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://lf.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ux.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://is.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ay.hnjuh.cn

[Q47] 与平均值比较
来源：http://ry.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://du.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://eg.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eh.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://bn.colortex.cn

[Q49] 更新单行
来源：http://yb.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ms.huixinmuqiang.cn

[Q50] 批量更新
来源：http://wr.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ks.9csxet.cn

[Q51] 用子查询更新
来源：http://bw.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hv.haigaiapp.cn

[Q52] 删除指定行
来源：http://go.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://vi.lnxyls.cn

[Q53] 按条件删除
来源：http://ba.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ai.huanxung.cn

[Q54] 清空表
来源：http://wc.szsharing.cn

TRUNCATE TABLE logs;
来源：http://tc.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://vs.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vf.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ca.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rh.huixinmuqiang.cn

[Q57] 行号
来源：http://rm.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ok.colortex.cn

[Q58] 累计求和
来源：http://yx.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tu.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://sw.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gq.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://ho.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bt.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wu.haigaiapp.cn

[Q61] 移动平均
来源：http://pb.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ta.521024.cn

[Q62] 分组占比
来源：http://gh.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vu.nszjky.cn


<!-- 参考信息 -->