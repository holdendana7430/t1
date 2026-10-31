代发 wailian999

PHP:  // 手写递归函数
来源：http://dj.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ay.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pq.huixinmuqiang.cn

Java: // 手写递归
来源：http://ph.newstarts.cn

Go:   // 手写递归
来源：http://ra.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kq.chemitech.net.cn

C#:   // 手写递归
来源：http://ds.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jb.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mh.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dk.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bl.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gw.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pc.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ik.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gn.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.nszjky.cn

================================================================================
来源：http://rj.asd995.cn

O. 并发与异步
来源：http://gs.haigaiapp.cn

================================================================================
来源：http://vg.521024.cn

[O01] 启动一个线程
来源：http://zd.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jx.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bd.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cy.jctech888.com.cn

TS:   // 同 JS
来源：http://iy.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://ei.szxytkj.cn

Go:   go f()
来源：http://sp.521024.cn

Ruby: Thread.new { f }
来源：http://tu.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://ha.wgjwhj.cn

[O02] 使用线程池
来源：http://rj.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hu.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jk.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://ux.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://ox.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ii.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wt.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tr.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aw.colortex.cn

[O03] 加锁保护共享数据
来源：http://kq.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://mu.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://yd.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ng.gzmigu.cn

TS:   // 同 JS
来源：http://cn.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://zg.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gu.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xk.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://qm.nszjky.cn

[O04] 定义异步函数并等待
来源：http://aw.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://xh.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mx.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://bm.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://du.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aj.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iv.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://de.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://ej.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://rr.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://oo.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mz.521024.cn

JS:   await Promise.all(tasks)
来源：http://mh.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://lx.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mn.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lw.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://vs.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ci.hahajie.cn

[O06] 使用进程池
来源：http://tf.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yx.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yu.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://dm.521024.cn

TS:   // child_process / cluster 模块
来源：http://xw.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xe.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kb.yuntaijiaju.cn

Ruby: // fork 块
来源：http://vx.wgjwhj.cn

C#:   Parallel.For
来源：http://rv.bjjhwx.cn

================================================================================
来源：http://yv.hahajie.cn

P. 常用工具函数
来源：http://jc.szxytkj.cn

================================================================================
来源：http://vt.colortex.cn

[P01] 生成 UUID
来源：http://zg.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://sg.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ln.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://xz.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://tc.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://mf.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://cg.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://gf.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://bk.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://qc.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ba.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nt.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cd.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mv.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xf.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ea.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sk.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pv.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://oa.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qk.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aj.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hn.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ca.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xk.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uy.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bd.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hg.9csxet.cn

[P04] 求长度
来源：http://zy.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tq.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sh.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cg.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wz.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://yy.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://lr.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://bn.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lf.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://sl.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gq.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ov.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yt.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vo.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cj.jctech888.com.cn

Ruby: a == b
来源：http://to.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rb.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rd.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hn.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://zl.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cg.yuexingan06.cn

TS:   if (x == null) {}
来源：http://dc.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qt.9csxet.cn

Go:   if x == nil {}
来源：http://ox.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vi.jctech888.com.cn

C#:   if (x is null) {}
来源：http://gg.521024.cn

[P07] 防抖与节流
来源：http://yq.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pg.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://kv.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dr.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sr.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cy.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gv.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zj.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oh.nszjky.cn

[P08] 处理浮点精度问题
来源：http://kl.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mo.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ho.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ue.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gn.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ui.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bx.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://za.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gh.jianghongdianzi.cn

================================================================================
来源：http://yz.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vl.nszjky.cn

================================================================================
来源：http://xz.jctech888.com.cn

[Q01] 创建表
来源：http://fs.shxzskj.cn

CREATE TABLE users (
来源：http://xn.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xv.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://hy.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://as.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wz.bookmarksfly.cn

);
来源：http://xl.lnxyls.cn

[Q02] 创建带外键的表
来源：http://nc.colortex.cn

CREATE TABLE orders (
来源：http://wt.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pn.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://bm.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://jc.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qz.colortex.cn

);
来源：http://ae.panjiajie.cn

[Q03] 增加列
来源：http://yq.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uf.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://zm.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tz.jctech888.com.cn

[Q05] 重命名列
来源：http://uv.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gb.huixiangedu.cn

[Q06] 删除列
来源：http://qm.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wt.jianghongdianzi.cn

[Q07] 删除表
来源：http://bp.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://vo.nszjky.cn

[Q08] 创建普通索引
来源：http://wb.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qc.hahajie.cn

[Q09] 创建唯一索引
来源：http://jq.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cc.nicolike.cn

[Q10] 插入单行
来源：http://du.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qd.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://ep.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mt.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://ev.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cn.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qf.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://iu.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ux.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://ur.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oi.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bx.nicolike.cn

[Q15] 查询全部
来源：http://nh.shtwfgs.cn

SELECT * FROM users;
来源：http://zl.chemitech.net.cn

[Q16] 查询指定列
来源：http://cg.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://os.nicolike.cn

[Q17] 条件查询
来源：http://cb.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://si.gzmigu.cn

[Q18] 模糊匹配
来源：http://su.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://po.shxzskj.cn

[Q19] 范围查询
来源：http://te.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hp.chemitech.net.cn

[Q20] IN 列表
来源：http://cy.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zx.bjjhwx.cn

[Q21] 空值判断
来源：http://xj.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iz.shtwfgs.cn

[Q22] 排序
来源：http://du.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dm.wgjwhj.cn

[Q23] 分页
来源：http://vb.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zz.huixiangedu.cn

[Q24] 去重
来源：http://wn.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://sw.9csxet.cn

[Q25] 只取前 N 条
来源：http://rr.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ne.haigaiapp.cn

[Q26] 计数
来源：http://ml.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://lw.9csxet.cn

[Q27] 条件计数
来源：http://qk.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qx.szxytkj.cn

[Q28] 求和与平均
来源：http://lf.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fo.bookmarksfly.cn

[Q29] 最大最小值
来源：http://oe.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uu.shxzskj.cn

[Q30] 分组统计
来源：http://xj.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pb.newstarts.cn

[Q31] 分组后过滤
来源：http://ky.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kz.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://gv.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dm.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qg.panjiajie.cn

[Q33] 多列分组
来源：http://oq.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uj.muxihuayi.cn

[Q34] 每组取第一条
来源：http://bu.shxzskj.cn

SELECT * FROM (
来源：http://gl.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xz.gzmigu.cn

) t WHERE rn = 1;
来源：http://fq.hahajie.cn

[Q35] 内连接
来源：http://dx.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sd.asd995.cn

[Q36] 左连接
来源：http://cz.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://so.huixiangedu.cn

[Q37] 右连接
来源：http://jj.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://er.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mq.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://se.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://wz.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fi.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://is.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://os.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zl.chemitech.net.cn

[Q41] 多表连接
来源：http://wt.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vt.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://rj.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://kv.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://dq.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://td.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sv.jctech888.com.cn

[Q43] 标量子查询
来源：http://ys.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hq.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://lk.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zi.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://uj.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uq.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://au.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gq.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://gh.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://so.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://gp.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gv.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://qi.shxzukj.cn

[Q49] 更新单行
来源：http://vf.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mn.hahajie.cn

[Q50] 批量更新
来源：http://bv.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jv.szsharing.cn

[Q51] 用子查询更新
来源：http://yd.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lf.asd995.cn

[Q52] 删除指定行
来源：http://xl.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://uc.bookmarksfly.cn

[Q53] 按条件删除
来源：http://ed.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hs.huixiangedu.cn

[Q54] 清空表
来源：http://zb.newstarts.cn

TRUNCATE TABLE logs;
来源：http://gp.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://fg.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xm.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://az.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://md.jianghongdianzi.cn

[Q57] 行号
来源：http://pi.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uq.yuntaijiaju.cn

[Q58] 累计求和
来源：http://lm.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pw.shtwfgs.cn

[Q59] 分组内累计
来源：http://jx.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dw.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://vh.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fb.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nn.nicolike.cn

[Q61] 移动平均
来源：http://pm.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dc.panjiajie.cn

[Q62] 分组占比
来源：http://oi.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uc.asd995.cn

[Q63] 开启事务
来源：http://yn.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fy.yuntaijiaju.cn

[Q64] 提交事务
来源：http://gp.wgjwhj.cn

COMMIT;
来源：http://pa.hahajie.cn


<!-- 参考信息 -->