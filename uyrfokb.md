代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://rs.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ey.521024.cn

[N11] 二叉树中序遍历
来源：http://fg.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ug.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://kg.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sn.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://al.bookmarksfly.cn

Java: // 手写递归
来源：http://fg.jctech888.com.cn

Go:   // 手写递归
来源：http://nv.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gh.shxzskj.cn

C#:   // 手写递归
来源：http://ho.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://am.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vr.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nf.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://at.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ns.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://py.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zy.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://es.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kr.hnjuh.cn

================================================================================
来源：http://aa.bjjhwx.cn

O. 并发与异步
来源：http://lo.9csxet.cn

================================================================================
来源：http://eh.hnjuh.cn

[O01] 启动一个线程
来源：http://nx.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sz.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ts.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://so.nszjky.cn

TS:   // 同 JS
来源：http://gp.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://mq.muxihuayi.cn

Go:   go f()
来源：http://pp.shxzskj.cn

Ruby: Thread.new { f }
来源：http://jp.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://uf.asd995.cn

[O02] 使用线程池
来源：http://me.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gh.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cx.nicolike.cn

JS:   // worker_threads 线程池
来源：http://ha.nicolike.cn

TS:   // worker_threads 线程池
来源：http://gs.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gm.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fw.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kk.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wa.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://gk.521024.cn

Py:   with lock: shared += 1
来源：http://vu.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://il.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pl.hnjuh.cn

TS:   // 同 JS
来源：http://fx.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ge.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cz.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kv.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://qt.asd995.cn

[O04] 定义异步函数并等待
来源：http://yw.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://lw.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vc.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://pu.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nz.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ef.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bi.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hq.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://pu.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://gk.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://pu.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rl.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://aq.asd995.cn

TS:   await Promise.all(tasks)
来源：http://yv.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ng.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ob.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://fv.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yb.bjjhwx.cn

[O06] 使用进程池
来源：http://hv.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ux.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ge.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://de.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://dh.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://af.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gl.muxihuayi.cn

Ruby: // fork 块
来源：http://hr.yuexingan06.cn

C#:   Parallel.For
来源：http://qs.bjjhwx.cn

================================================================================
来源：http://rv.shtwfgs.cn

P. 常用工具函数
来源：http://xj.lnxyls.cn

================================================================================
来源：http://os.bookmarksfly.cn

[P01] 生成 UUID
来源：http://hh.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://lk.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jp.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://av.hahajie.cn

TS:   crypto.randomUUID()
来源：http://hd.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://ts.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://tx.colortex.cn

Ruby: SecureRandom.uuid
来源：http://rr.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://ju.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ju.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lt.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ot.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ic.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wg.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bl.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lv.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qh.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ei.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://an.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fb.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ld.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oh.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://or.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jr.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aa.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jw.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xz.521024.cn

[P04] 求长度
来源：http://fm.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nf.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rl.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://np.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kn.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://cf.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://zp.hnjuh.cn

Ruby: x.length;  x.size
来源：http://rf.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kc.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://ri.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gv.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pq.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xe.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vb.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://re.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ew.shxzukj.cn

Ruby: a == b
来源：http://hq.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lz.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hp.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yb.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://dd.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sv.9csxet.cn

TS:   if (x == null) {}
来源：http://sd.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hl.521024.cn

Go:   if x == nil {}
来源：http://vy.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vc.shtwfgs.cn

C#:   if (x is null) {}
来源：http://wa.muxihuayi.cn

[P07] 防抖与节流
来源：http://yh.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pe.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://kr.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ea.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qe.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pq.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dg.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lp.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cq.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://nr.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xg.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mj.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yw.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://as.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fl.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mz.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zb.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jx.szsharing.cn

================================================================================
来源：http://ft.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ni.szxytkj.cn

================================================================================
来源：http://xj.huixiangedu.cn

[Q01] 创建表
来源：http://id.szxytkj.cn

CREATE TABLE users (
来源：http://zw.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ve.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://qf.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://pu.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ug.yuntaijiaju.cn

);
来源：http://pn.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://qu.szsharing.cn

CREATE TABLE orders (
来源：http://tl.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cy.wgjwhj.cn

user_id INT NOT NULL,
来源：http://jh.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://dq.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gk.wgjwhj.cn

);
来源：http://ks.panjiajie.cn

[Q03] 增加列
来源：http://ae.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://de.shxzukj.cn

[Q04] 修改列类型
来源：http://od.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jl.szsharing.cn

[Q05] 重命名列
来源：http://kr.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://om.nicolike.cn

[Q06] 删除列
来源：http://uj.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://es.newstarts.cn

[Q07] 删除表
来源：http://gn.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://rj.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://eq.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fc.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://va.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xn.lnxyls.cn

[Q10] 插入单行
来源：http://tt.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cl.shtwfgs.cn

[Q11] 一次插入多行
来源：http://dh.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ib.521024.cn

[Q12] 插入后取自增 ID
来源：http://xl.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ng.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ba.huanxung.cn

[Q13] 忽略重复插入
来源：http://ca.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xz.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://sw.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://we.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qd.shxzskj.cn

[Q15] 查询全部
来源：http://li.521024.cn

SELECT * FROM users;
来源：http://rk.wgjwhj.cn

[Q16] 查询指定列
来源：http://jc.gzmigu.cn

SELECT id, name FROM users;
来源：http://qa.yuexingan06.cn

[Q17] 条件查询
来源：http://kq.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kv.huanxung.cn

[Q18] 模糊匹配
来源：http://ir.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://up.colortex.cn

[Q19] 范围查询
来源：http://ym.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wx.jctech888.com.cn

[Q20] IN 列表
来源：http://sm.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pt.shxzukj.cn

[Q21] 空值判断
来源：http://tf.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://og.9csxet.cn

[Q22] 排序
来源：http://xv.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nu.asd995.cn

[Q23] 分页
来源：http://bl.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hk.shxzskj.cn

[Q24] 去重
来源：http://vj.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://xk.panjiajie.cn

[Q25] 只取前 N 条
来源：http://ka.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ln.huixinmuqiang.cn

[Q26] 计数
来源：http://nf.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://qc.huixinmuqiang.cn

[Q27] 条件计数
来源：http://nz.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zp.shxzukj.cn

[Q28] 求和与平均
来源：http://gn.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yn.bjjhwx.cn

[Q29] 最大最小值
来源：http://ny.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dl.gzmigu.cn

[Q30] 分组统计
来源：http://ol.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gz.muxihuayi.cn

[Q31] 分组后过滤
来源：http://xk.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rn.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://sj.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jo.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ij.newstarts.cn

[Q33] 多列分组
来源：http://zf.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dx.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://ki.haigaiapp.cn

SELECT * FROM (
来源：http://zb.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qd.shxzskj.cn

) t WHERE rn = 1;
来源：http://cd.haigaiapp.cn

[Q35] 内连接
来源：http://xf.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fv.colortex.cn

[Q36] 左连接
来源：http://iy.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hn.wgjwhj.cn

[Q37] 右连接
来源：http://ku.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mp.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kb.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ff.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://na.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tr.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ze.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fq.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://er.colortex.cn

[Q41] 多表连接
来源：http://ky.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://aa.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://tw.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://pq.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://sq.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://ps.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ya.colortex.cn

[Q43] 标量子查询
来源：http://og.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://av.bjjhwx.cn

[Q44] IN 子查询
来源：http://do.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mv.asd995.cn

[Q45] EXISTS 判断存在
来源：http://dr.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mn.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rs.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://og.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ky.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fe.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://by.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hk.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://oo.wgjwhj.cn

[Q49] 更新单行
来源：http://sq.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bn.huixiangedu.cn

[Q50] 批量更新
来源：http://tn.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pe.yuexingan06.cn

[Q51] 用子查询更新
来源：http://zh.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ip.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://em.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://oy.bjjhwx.cn

[Q53] 按条件删除
来源：http://ez.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pj.szxytkj.cn

[Q54] 清空表
来源：http://sp.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://zd.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://ub.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://an.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://rd.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ob.newstarts.cn

[Q57] 行号
来源：http://ul.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://df.shxzukj.cn

[Q58] 累计求和
来源：http://in.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lc.521024.cn

[Q59] 分组内累计
来源：http://ih.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uq.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://qr.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ec.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uv.jianghongdianzi.cn

[Q61] 移动平均
来源：http://cf.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bn.yuntaijiaju.cn

[Q62] 分组占比
来源：http://yg.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qt.bookmarksfly.cn


<!-- 参考信息 -->