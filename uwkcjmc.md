代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nx.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yl.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wm.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ja.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ff.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tp.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cy.haigaiapp.cn

================================================================================
来源：http://kx.nicolike.cn

O. 并发与异步
来源：http://gd.huixinmuqiang.cn

================================================================================
来源：http://dq.lnxyls.cn

[O01] 启动一个线程
来源：http://vj.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wm.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dt.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gn.szxytkj.cn

TS:   // 同 JS
来源：http://kq.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ln.shxzukj.cn

Go:   go f()
来源：http://gh.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://sa.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://eb.521024.cn

[O02] 使用线程池
来源：http://dt.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fr.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kp.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ac.9csxet.cn

TS:   // worker_threads 线程池
来源：http://mt.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ej.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sq.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xw.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cr.9csxet.cn

[O03] 加锁保护共享数据
来源：http://ey.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://ut.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://sg.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://de.521024.cn

TS:   // 同 JS
来源：http://uy.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://pv.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lj.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vy.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://jl.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://qo.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://io.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ba.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ty.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zi.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xb.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kg.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fq.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://hm.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://hp.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://at.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tw.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://gl.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://kb.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hr.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hm.newstarts.cn

Ruby: threads.map(&:join)
来源：http://ta.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cn.yuntaijiaju.cn

[O06] 使用进程池
来源：http://nz.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pj.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://il.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://bb.521024.cn

TS:   // child_process / cluster 模块
来源：http://vm.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tn.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uf.chemitech.net.cn

Ruby: // fork 块
来源：http://ev.panjiajie.cn

C#:   Parallel.For
来源：http://ns.gzmigu.cn

================================================================================
来源：http://ty.colortex.cn

P. 常用工具函数
来源：http://vs.szsharing.cn

================================================================================
来源：http://kf.bjjhwx.cn

[P01] 生成 UUID
来源：http://fz.colortex.cn

Py:   str(uuid.uuid4())
来源：http://kg.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fa.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://gp.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://tn.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://cd.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://vt.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://ym.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://mp.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://by.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://np.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zz.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yt.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tg.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yd.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pz.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ll.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ta.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://wp.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kb.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vc.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://td.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eh.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mf.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://we.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uz.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ak.nicolike.cn

[P04] 求长度
来源：http://pj.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fv.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cn.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jf.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uw.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://bd.szsharing.cn

Go:   len(arr);  len(m)
来源：http://yy.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://vg.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vv.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://dq.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ew.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dl.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lb.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://db.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://am.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://is.colortex.cn

Ruby: a == b
来源：http://ei.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://po.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gh.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ex.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://dv.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://js.shtwfgs.cn

TS:   if (x == null) {}
来源：http://kp.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ij.nicolike.cn

Go:   if x == nil {}
来源：http://vm.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uf.huanxung.cn

C#:   if (x is null) {}
来源：http://bm.lnxyls.cn

[P07] 防抖与节流
来源：http://da.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://en.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://gw.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oz.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ri.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://us.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ra.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ne.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ht.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://zf.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://an.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pw.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vi.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vm.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xx.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yi.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mq.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ew.colortex.cn

================================================================================
来源：http://my.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ak.muxihuayi.cn

================================================================================
来源：http://vb.yuexingan06.cn

[Q01] 创建表
来源：http://rm.shtwfgs.cn

CREATE TABLE users (
来源：http://lp.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bs.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://oo.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://vl.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rp.muxihuayi.cn

);
来源：http://mv.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://ef.szsharing.cn

CREATE TABLE orders (
来源：http://pt.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qa.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://jp.huanxung.cn

amount DECIMAL(10, 2),
来源：http://nu.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tg.szxytkj.cn

);
来源：http://zp.nicolike.cn

[Q03] 增加列
来源：http://qc.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tj.shxzukj.cn

[Q04] 修改列类型
来源：http://cf.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vf.bjjhwx.cn

[Q05] 重命名列
来源：http://kf.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ao.9csxet.cn

[Q06] 删除列
来源：http://vx.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hm.jianghongdianzi.cn

[Q07] 删除表
来源：http://ca.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://gb.panjiajie.cn

[Q08] 创建普通索引
来源：http://bj.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mt.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://ba.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://py.szsharing.cn

[Q10] 插入单行
来源：http://si.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://er.szsharing.cn

[Q11] 一次插入多行
来源：http://ru.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lw.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://bj.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iu.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zz.521024.cn

[Q13] 忽略重复插入
来源：http://xt.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aw.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://fn.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ub.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://di.newstarts.cn

[Q15] 查询全部
来源：http://wy.huanxung.cn

SELECT * FROM users;
来源：http://ae.huanxung.cn

[Q16] 查询指定列
来源：http://kg.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://jp.shxzskj.cn

[Q17] 条件查询
来源：http://ww.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zi.huixiangedu.cn

[Q18] 模糊匹配
来源：http://pk.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gt.colortex.cn

[Q19] 范围查询
来源：http://hr.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hy.jianghongdianzi.cn

[Q20] IN 列表
来源：http://mg.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xf.wgjwhj.cn

[Q21] 空值判断
来源：http://ja.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fv.wgjwhj.cn

[Q22] 排序
来源：http://ij.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wb.wgjwhj.cn

[Q23] 分页
来源：http://po.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://im.muxihuayi.cn

[Q24] 去重
来源：http://hn.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://ap.newstarts.cn

[Q25] 只取前 N 条
来源：http://kn.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yf.huanxung.cn

[Q26] 计数
来源：http://yq.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://lb.shxzskj.cn

[Q27] 条件计数
来源：http://nt.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://in.9csxet.cn

[Q28] 求和与平均
来源：http://da.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vo.muxihuayi.cn

[Q29] 最大最小值
来源：http://hm.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sf.nicolike.cn

[Q30] 分组统计
来源：http://ya.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hk.bjjhwx.cn

[Q31] 分组后过滤
来源：http://ln.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fn.521024.cn

[Q32] 分组拼接字符串
来源：http://fi.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sp.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ls.bookmarksfly.cn

[Q33] 多列分组
来源：http://xq.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cl.lnxyls.cn

[Q34] 每组取第一条
来源：http://lh.wgjwhj.cn

SELECT * FROM (
来源：http://op.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vm.huixiangedu.cn

) t WHERE rn = 1;
来源：http://mf.gzmigu.cn

[Q35] 内连接
来源：http://hx.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ea.panjiajie.cn

[Q36] 左连接
来源：http://gz.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ta.szsharing.cn

[Q37] 右连接
来源：http://jx.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ho.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://my.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ng.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://le.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zu.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rc.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sn.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yo.szsharing.cn

[Q41] 多表连接
来源：http://tw.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://es.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://le.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://gn.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://fj.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://bo.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hw.yuexingan06.cn

[Q43] 标量子查询
来源：http://qb.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xq.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://gk.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://og.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://eg.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nm.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hc.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bb.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://hj.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xl.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://za.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dm.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://pr.lnxyls.cn

[Q49] 更新单行
来源：http://kc.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oh.bookmarksfly.cn

[Q50] 批量更新
来源：http://xe.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yw.haigaiapp.cn

[Q51] 用子查询更新
来源：http://al.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qo.huanxung.cn

[Q52] 删除指定行
来源：http://pv.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://na.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://zg.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zq.yuexingan06.cn

[Q54] 清空表
来源：http://xp.nicolike.cn

TRUNCATE TABLE logs;
来源：http://yf.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://sa.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mf.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ws.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://se.gzmigu.cn

[Q57] 行号
来源：http://yy.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jh.wgjwhj.cn

[Q58] 累计求和
来源：http://jg.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gn.huanxung.cn

[Q59] 分组内累计
来源：http://hg.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://er.521024.cn

[Q60] 取上一行 / 下一行
来源：http://kr.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ml.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lp.nszjky.cn

[Q61] 移动平均
来源：http://vz.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ci.haigaiapp.cn

[Q62] 分组占比
来源：http://ik.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rt.bookmarksfly.cn

[Q63] 开启事务
来源：http://dp.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gl.nszjky.cn

[Q64] 提交事务
来源：http://nc.huixiangedu.cn

COMMIT;
来源：http://xi.nicolike.cn

[Q65] 回滚事务
来源：http://mh.yuexingan06.cn

ROLLBACK;
来源：http://bn.521024.cn

[Q66] 行锁查询
来源：http://am.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://im.asd995.cn

[Q67] 设置隔离级别
来源：http://yz.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bw.chemitech.net.cn

[Q68] 保存点
来源：http://zr.gzmigu.cn

SAVEPOINT sp1;
来源：http://uu.chemitech.net.cn


<!-- 参考信息 -->