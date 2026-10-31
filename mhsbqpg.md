代发 wailian999

Go:   // 手写递归
来源：http://it.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ey.haigaiapp.cn

C#:   // 手写递归
来源：http://lb.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xb.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yl.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gd.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gv.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qu.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jn.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qa.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mq.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tt.haigaiapp.cn

================================================================================
来源：http://gd.nicolike.cn

O. 并发与异步
来源：http://nq.521024.cn

================================================================================
来源：http://vd.lnxyls.cn

[O01] 启动一个线程
来源：http://wk.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jy.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jh.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vv.lnxyls.cn

TS:   // 同 JS
来源：http://fk.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://rs.hahajie.cn

Go:   go f()
来源：http://ez.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://jj.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://fi.shxzukj.cn

[O02] 使用线程池
来源：http://rt.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mw.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zo.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://sp.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://lj.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xw.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cq.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pr.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mo.newstarts.cn

[O03] 加锁保护共享数据
来源：http://mj.hnjuh.cn

Py:   with lock: shared += 1
来源：http://qx.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://dt.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rv.huixiangedu.cn

TS:   // 同 JS
来源：http://pa.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://wp.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ql.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tw.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://qx.hahajie.cn

[O04] 定义异步函数并等待
来源：http://df.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://yl.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://be.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://md.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pj.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wn.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zv.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ai.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ga.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://kx.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://fx.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://la.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://dm.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://bt.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zt.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bj.nicolike.cn

Ruby: threads.map(&:join)
来源：http://ph.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sg.jctech888.com.cn

[O06] 使用进程池
来源：http://ii.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jh.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bz.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://rt.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://jz.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://un.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hl.nszjky.cn

Ruby: // fork 块
来源：http://ev.huanxung.cn

C#:   Parallel.For
来源：http://wl.shxzukj.cn

================================================================================
来源：http://jz.shxzukj.cn

P. 常用工具函数
来源：http://kk.shxzukj.cn

================================================================================
来源：http://wo.shtwfgs.cn

[P01] 生成 UUID
来源：http://zv.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ln.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vt.huanxung.cn

JS:   crypto.randomUUID()
来源：http://qi.asd995.cn

TS:   crypto.randomUUID()
来源：http://pi.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://dw.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://dy.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://ho.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://ix.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://vp.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mc.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wn.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nj.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gw.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hn.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eo.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vo.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ym.lnxyls.cn

[P03] 生成短随机字符串
来源：http://ma.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ha.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://km.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cx.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mh.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bc.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rb.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wy.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mc.huixinmuqiang.cn

[P04] 求长度
来源：http://yu.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jd.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vp.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lq.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nl.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://pu.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://vt.shxzukj.cn

Ruby: x.length;  x.size
来源：http://nr.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dm.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://hg.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://am.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pf.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gl.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xz.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kl.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kx.colortex.cn

Ruby: a == b
来源：http://cv.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nh.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ge.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tj.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://hl.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xn.hnjuh.cn

TS:   if (x == null) {}
来源：http://lr.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eu.9csxet.cn

Go:   if x == nil {}
来源：http://ny.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hg.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://tb.nicolike.cn

[P07] 防抖与节流
来源：http://db.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yr.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://vf.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sx.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ii.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bh.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://er.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vj.asd995.cn

[P08] 处理浮点精度问题
来源：http://mq.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gj.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vx.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cn.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lp.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tv.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gi.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hh.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://md.9csxet.cn

================================================================================
来源：http://lg.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zg.jctech888.com.cn

================================================================================
来源：http://lh.gzmigu.cn

[Q01] 创建表
来源：http://vs.shxzskj.cn

CREATE TABLE users (
来源：http://rp.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ev.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://wq.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://wm.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lz.wgjwhj.cn

);
来源：http://kv.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ie.huanxung.cn

CREATE TABLE orders (
来源：http://ol.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://za.huanxung.cn

user_id INT NOT NULL,
来源：http://no.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://pu.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://je.hnjuh.cn

);
来源：http://se.bookmarksfly.cn

[Q03] 增加列
来源：http://ns.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://so.yuexingan06.cn

[Q04] 修改列类型
来源：http://vk.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://go.colortex.cn

[Q05] 重命名列
来源：http://xt.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nq.bookmarksfly.cn

[Q06] 删除列
来源：http://so.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nc.shxzskj.cn

[Q07] 删除表
来源：http://xr.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://mc.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://ni.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qf.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://gz.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gi.jctech888.com.cn

[Q10] 插入单行
来源：http://kj.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ed.asd995.cn

[Q11] 一次插入多行
来源：http://yh.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iv.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://xu.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pj.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ga.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://yn.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gx.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://xj.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qc.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ok.colortex.cn

[Q15] 查询全部
来源：http://hx.huanxung.cn

SELECT * FROM users;
来源：http://ox.szsharing.cn

[Q16] 查询指定列
来源：http://wi.colortex.cn

SELECT id, name FROM users;
来源：http://lg.shxzskj.cn

[Q17] 条件查询
来源：http://dq.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fb.521024.cn

[Q18] 模糊匹配
来源：http://vm.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hx.yuexingan06.cn

[Q19] 范围查询
来源：http://om.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yo.yuntaijiaju.cn

[Q20] IN 列表
来源：http://ly.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oo.colortex.cn

[Q21] 空值判断
来源：http://zg.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://va.chemitech.net.cn

[Q22] 排序
来源：http://mm.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bk.9csxet.cn

[Q23] 分页
来源：http://ki.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zl.huixinmuqiang.cn

[Q24] 去重
来源：http://ka.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://cd.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://zo.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ux.lnxyls.cn

[Q26] 计数
来源：http://jj.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://wc.szsharing.cn

[Q27] 条件计数
来源：http://ik.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iv.huixiangedu.cn

[Q28] 求和与平均
来源：http://zo.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bc.gzmigu.cn

[Q29] 最大最小值
来源：http://cc.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gs.huixinmuqiang.cn

[Q30] 分组统计
来源：http://at.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://it.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://oe.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sx.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://xx.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://il.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ao.szxytkj.cn

[Q33] 多列分组
来源：http://gz.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fh.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://kk.szxytkj.cn

SELECT * FROM (
来源：http://yu.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vs.shxzskj.cn

) t WHERE rn = 1;
来源：http://ug.haigaiapp.cn

[Q35] 内连接
来源：http://ot.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aq.9csxet.cn

[Q36] 左连接
来源：http://me.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nq.panjiajie.cn

[Q37] 右连接
来源：http://uu.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bi.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fv.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vq.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://gk.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ym.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yj.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://la.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bv.haigaiapp.cn

[Q41] 多表连接
来源：http://rx.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ui.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://lw.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://cd.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://gg.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://je.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ga.asd995.cn

[Q43] 标量子查询
来源：http://qr.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://km.521024.cn

[Q44] IN 子查询
来源：http://oq.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wy.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ec.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fn.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zd.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fk.haigaiapp.cn

[Q47] 与平均值比较
来源：http://ll.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pf.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://gh.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eg.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://yr.lnxyls.cn

[Q49] 更新单行
来源：http://za.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fk.szxytkj.cn

[Q50] 批量更新
来源：http://bp.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kl.colortex.cn

[Q51] 用子查询更新
来源：http://re.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qn.szsharing.cn

[Q52] 删除指定行
来源：http://yd.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://qo.huixiangedu.cn

[Q53] 按条件删除
来源：http://lf.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://va.hahajie.cn

[Q54] 清空表
来源：http://zh.9csxet.cn

TRUNCATE TABLE logs;
来源：http://ie.szsharing.cn

[Q55] 排名（并列占位）
来源：http://sx.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gf.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://ls.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tr.hnjuh.cn

[Q57] 行号
来源：http://qu.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ay.nicolike.cn

[Q58] 累计求和
来源：http://ia.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://la.bjjhwx.cn

[Q59] 分组内累计
来源：http://rm.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xa.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://xw.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iy.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jp.gzmigu.cn

[Q61] 移动平均
来源：http://nr.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cd.9csxet.cn

[Q62] 分组占比
来源：http://cv.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qh.wgjwhj.cn

[Q63] 开启事务
来源：http://gf.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xl.szxytkj.cn

[Q64] 提交事务
来源：http://yv.jctech888.com.cn

COMMIT;
来源：http://fk.shxzukj.cn

[Q65] 回滚事务
来源：http://bh.yuntaijiaju.cn

ROLLBACK;
来源：http://vb.nszjky.cn

[Q66] 行锁查询
来源：http://ur.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mo.szxytkj.cn


<!-- 参考信息 -->