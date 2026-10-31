代发 wailian999

Go:   // 手写递归
来源：http://nl.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ev.9csxet.cn

C#:   // 手写递归
来源：http://wx.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wl.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xr.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tz.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yy.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nq.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://io.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hm.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sb.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://he.jctech888.com.cn

================================================================================
来源：http://bw.nszjky.cn

O. 并发与异步
来源：http://bi.haigaiapp.cn

================================================================================
来源：http://cs.yuexingan06.cn

[O01] 启动一个线程
来源：http://qu.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tj.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jr.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lm.yuntaijiaju.cn

TS:   // 同 JS
来源：http://nf.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://du.hahajie.cn

Go:   go f()
来源：http://cs.lnxyls.cn

Ruby: Thread.new { f }
来源：http://gh.521024.cn

C#:   Task.Run(() => F());
来源：http://vd.jianghongdianzi.cn

[O02] 使用线程池
来源：http://iz.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yq.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ga.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://jm.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://ek.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rc.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tb.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mq.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xa.nicolike.cn

[O03] 加锁保护共享数据
来源：http://tc.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://xc.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fk.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ek.nszjky.cn

TS:   // 同 JS
来源：http://ki.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://lu.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ci.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nw.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://gq.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://tm.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://pp.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ko.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://tv.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fa.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ze.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pn.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wg.asd995.cn

C#:   async Task F() { await G(); }
来源：http://ie.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://il.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://dy.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xh.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://lt.asd995.cn

TS:   await Promise.all(tasks)
来源：http://wf.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hw.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ye.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://hf.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://py.huixinmuqiang.cn

[O06] 使用进程池
来源：http://fe.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://td.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pt.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://bu.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://nq.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mp.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://un.shxzukj.cn

Ruby: // fork 块
来源：http://bf.asd995.cn

C#:   Parallel.For
来源：http://mz.hnjuh.cn

================================================================================
来源：http://dz.hnjuh.cn

P. 常用工具函数
来源：http://dt.panjiajie.cn

================================================================================
来源：http://nk.hnjuh.cn

[P01] 生成 UUID
来源：http://uf.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://iq.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ev.asd995.cn

JS:   crypto.randomUUID()
来源：http://ww.nicolike.cn

TS:   crypto.randomUUID()
来源：http://ww.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://wn.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://ad.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://bc.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://vo.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://xz.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gq.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nu.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xq.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uu.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xw.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://np.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://id.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xt.huanxung.cn

[P03] 生成短随机字符串
来源：http://qi.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://il.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kg.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xw.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aj.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xg.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cy.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ki.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://it.shtwfgs.cn

[P04] 求长度
来源：http://qj.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gs.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ss.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vx.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sh.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://ep.asd995.cn

Go:   len(arr);  len(m)
来源：http://cp.shxzukj.cn

Ruby: x.length;  x.size
来源：http://cr.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fw.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://ml.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sg.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pu.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zg.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yv.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qe.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ax.asd995.cn

Ruby: a == b
来源：http://rp.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uz.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ju.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kn.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://co.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lv.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://uy.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oo.521024.cn

Go:   if x == nil {}
来源：http://io.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wi.yuexingan06.cn

C#:   if (x is null) {}
来源：http://fh.chemitech.net.cn

[P07] 防抖与节流
来源：http://cc.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jw.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://di.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hj.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wt.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vb.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bv.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ds.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wq.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://if.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ua.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tv.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hx.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tq.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xp.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cf.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jp.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yv.panjiajie.cn

================================================================================
来源：http://ak.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ir.lnxyls.cn

================================================================================
来源：http://lo.haigaiapp.cn

[Q01] 创建表
来源：http://xh.huixiangedu.cn

CREATE TABLE users (
来源：http://pa.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xk.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://al.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://ys.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://to.yuexingan06.cn

);
来源：http://qa.9csxet.cn

[Q02] 创建带外键的表
来源：http://le.nicolike.cn

CREATE TABLE orders (
来源：http://vf.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cw.gzmigu.cn

user_id INT NOT NULL,
来源：http://cc.newstarts.cn

amount DECIMAL(10, 2),
来源：http://or.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cz.shxzskj.cn

);
来源：http://ey.shxzskj.cn

[Q03] 增加列
来源：http://ws.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gd.bookmarksfly.cn

[Q04] 修改列类型
来源：http://jh.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ss.huixiangedu.cn

[Q05] 重命名列
来源：http://xo.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mb.521024.cn

[Q06] 删除列
来源：http://mt.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gx.huanxung.cn

[Q07] 删除表
来源：http://te.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://hx.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://cl.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fc.9csxet.cn

[Q09] 创建唯一索引
来源：http://ix.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lm.521024.cn

[Q10] 插入单行
来源：http://su.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vb.newstarts.cn

[Q11] 一次插入多行
来源：http://ii.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mt.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://cl.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rj.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pc.szxytkj.cn

[Q13] 忽略重复插入
来源：http://tv.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://to.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://pa.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yt.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qm.muxihuayi.cn

[Q15] 查询全部
来源：http://qb.shxzukj.cn

SELECT * FROM users;
来源：http://qv.bjjhwx.cn

[Q16] 查询指定列
来源：http://ed.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://hg.huixinmuqiang.cn

[Q17] 条件查询
来源：http://pw.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lk.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://up.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hw.shxzukj.cn

[Q19] 范围查询
来源：http://qt.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wu.huixinmuqiang.cn

[Q20] IN 列表
来源：http://op.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ia.wgjwhj.cn

[Q21] 空值判断
来源：http://wl.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rl.chemitech.net.cn

[Q22] 排序
来源：http://rc.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ox.jianghongdianzi.cn

[Q23] 分页
来源：http://xo.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yn.huanxung.cn

[Q24] 去重
来源：http://kt.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://wu.szsharing.cn

[Q25] 只取前 N 条
来源：http://ay.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jo.muxihuayi.cn

[Q26] 计数
来源：http://di.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://kn.szxytkj.cn

[Q27] 条件计数
来源：http://iz.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rm.yuexingan06.cn

[Q28] 求和与平均
来源：http://fs.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gu.nszjky.cn

[Q29] 最大最小值
来源：http://cq.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wh.shxzukj.cn

[Q30] 分组统计
来源：http://nc.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qj.9csxet.cn

[Q31] 分组后过滤
来源：http://ai.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qm.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://vt.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ga.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://is.huixinmuqiang.cn

[Q33] 多列分组
来源：http://uq.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gj.jctech888.com.cn

[Q34] 每组取第一条
来源：http://nn.nszjky.cn

SELECT * FROM (
来源：http://zc.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rz.muxihuayi.cn

) t WHERE rn = 1;
来源：http://dl.szxytkj.cn

[Q35] 内连接
来源：http://de.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ty.jctech888.com.cn

[Q36] 左连接
来源：http://zm.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ul.shxzskj.cn

[Q37] 右连接
来源：http://oc.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fm.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wd.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gt.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://zk.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ip.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ac.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fp.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ad.huixiangedu.cn

[Q41] 多表连接
来源：http://kp.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fb.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://ay.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://nc.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://fy.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://gj.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qo.haigaiapp.cn

[Q43] 标量子查询
来源：http://fa.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sz.muxihuayi.cn

[Q44] IN 子查询
来源：http://be.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://se.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://tn.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uy.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lt.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xq.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://sm.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://km.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://vk.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ao.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ax.jctech888.com.cn

[Q49] 更新单行
来源：http://ds.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://al.bjjhwx.cn

[Q50] 批量更新
来源：http://jz.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zm.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://uh.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uq.hnjuh.cn

[Q52] 删除指定行
来源：http://be.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://rp.bjjhwx.cn

[Q53] 按条件删除
来源：http://gm.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ie.muxihuayi.cn

[Q54] 清空表
来源：http://ki.nicolike.cn

TRUNCATE TABLE logs;
来源：http://nd.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://xy.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yo.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://kh.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ur.nszjky.cn

[Q57] 行号
来源：http://kx.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dp.bjjhwx.cn

[Q58] 累计求和
来源：http://pz.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xu.gzmigu.cn

[Q59] 分组内累计
来源：http://qb.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eb.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://zd.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fj.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.asd995.cn

[Q61] 移动平均
来源：http://ji.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cs.szxytkj.cn

[Q62] 分组占比
来源：http://fc.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vc.szxytkj.cn

[Q63] 开启事务
来源：http://zp.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uu.yuntaijiaju.cn

[Q64] 提交事务
来源：http://mm.newstarts.cn

COMMIT;
来源：http://of.huixiangedu.cn

[Q65] 回滚事务
来源：http://ns.yuexingan06.cn

ROLLBACK;
来源：http://fr.bookmarksfly.cn

[Q66] 行锁查询
来源：http://hz.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lq.shxzskj.cn


<!-- 参考信息 -->