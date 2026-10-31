代发 wailian999

Go:   // 手写递归
来源：http://zq.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ew.9csxet.cn

C#:   // 手写递归
来源：http://ek.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yo.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xp.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zt.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zu.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jl.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ri.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://we.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pn.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bg.hnjuh.cn

================================================================================
来源：http://dl.521024.cn

O. 并发与异步
来源：http://lb.yuntaijiaju.cn

================================================================================
来源：http://hy.newstarts.cn

[O01] 启动一个线程
来源：http://kg.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xc.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cr.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dl.nszjky.cn

TS:   // 同 JS
来源：http://th.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://lg.gzmigu.cn

Go:   go f()
来源：http://sp.nszjky.cn

Ruby: Thread.new { f }
来源：http://mt.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://sn.hnjuh.cn

[O02] 使用线程池
来源：http://zy.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zd.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tm.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://ml.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://jn.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zp.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ps.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jw.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pn.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ct.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://am.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://np.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zr.bookmarksfly.cn

TS:   // 同 JS
来源：http://ma.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://ro.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rv.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kw.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://nc.asd995.cn

[O04] 定义异步函数并等待
来源：http://zn.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://ey.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vj.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://eh.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tv.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ch.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kd.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://em.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://wn.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://wf.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://cs.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ro.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://by.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://ej.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rm.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ad.newstarts.cn

Ruby: threads.map(&:join)
来源：http://gd.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pn.huixinmuqiang.cn

[O06] 使用进程池
来源：http://xi.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mp.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ja.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://vd.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://rg.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wk.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lu.9csxet.cn

Ruby: // fork 块
来源：http://zn.szsharing.cn

C#:   Parallel.For
来源：http://bp.huanxung.cn

================================================================================
来源：http://lp.huixinmuqiang.cn

P. 常用工具函数
来源：http://sz.jianghongdianzi.cn

================================================================================
来源：http://vl.wgjwhj.cn

[P01] 生成 UUID
来源：http://fc.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://ro.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cp.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://ia.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://jn.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://lr.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://uz.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://mp.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://fx.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://oi.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ww.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wm.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gy.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ya.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qn.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cf.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zp.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kw.hahajie.cn

[P03] 生成短随机字符串
来源：http://tf.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jj.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gs.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gp.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ko.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ur.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cf.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kh.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ym.shtwfgs.cn

[P04] 求长度
来源：http://sv.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pt.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://of.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cl.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ey.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://nz.newstarts.cn

Go:   len(arr);  len(m)
来源：http://cv.huanxung.cn

Ruby: x.length;  x.size
来源：http://qp.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bj.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://kp.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uk.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nr.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fx.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ck.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ho.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ru.asd995.cn

Ruby: a == b
来源：http://te.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wg.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tq.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://do.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://km.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ns.szsharing.cn

TS:   if (x == null) {}
来源：http://it.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xe.wgjwhj.cn

Go:   if x == nil {}
来源：http://qh.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://om.shxzukj.cn

C#:   if (x is null) {}
来源：http://oa.shtwfgs.cn

[P07] 防抖与节流
来源：http://jc.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jr.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://mi.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rh.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iy.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vf.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xz.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qy.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://he.nszjky.cn

[P08] 处理浮点精度问题
来源：http://kw.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hf.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hd.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ak.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yb.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fq.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jc.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cr.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fm.shxzukj.cn

================================================================================
来源：http://es.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hd.muxihuayi.cn

================================================================================
来源：http://zu.huixiangedu.cn

[Q01] 创建表
来源：http://jh.shxzskj.cn

CREATE TABLE users (
来源：http://ew.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dc.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ki.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://ka.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jr.huixiangedu.cn

);
来源：http://om.nszjky.cn

[Q02] 创建带外键的表
来源：http://ow.szsharing.cn

CREATE TABLE orders (
来源：http://uj.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tg.wgjwhj.cn

user_id INT NOT NULL,
来源：http://ax.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://ax.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nq.shxzskj.cn

);
来源：http://ye.panjiajie.cn

[Q03] 增加列
来源：http://ci.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://on.panjiajie.cn

[Q04] 修改列类型
来源：http://np.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://se.shxzukj.cn

[Q05] 重命名列
来源：http://vw.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vm.9csxet.cn

[Q06] 删除列
来源：http://jp.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vh.shxzskj.cn

[Q07] 删除表
来源：http://ev.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://mc.chemitech.net.cn

[Q08] 创建普通索引
来源：http://re.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ds.panjiajie.cn

[Q09] 创建唯一索引
来源：http://ne.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xt.shxzskj.cn

[Q10] 插入单行
来源：http://mu.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zi.shxzukj.cn

[Q11] 一次插入多行
来源：http://ao.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hs.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://zu.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://im.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kx.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://sd.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zj.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://em.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mh.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ut.huixiangedu.cn

[Q15] 查询全部
来源：http://nt.huanxung.cn

SELECT * FROM users;
来源：http://fd.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://wq.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://vf.shxzskj.cn

[Q17] 条件查询
来源：http://nv.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oh.521024.cn

[Q18] 模糊匹配
来源：http://zw.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mj.nszjky.cn

[Q19] 范围查询
来源：http://nw.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xo.huixinmuqiang.cn

[Q20] IN 列表
来源：http://yj.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pk.szxytkj.cn

[Q21] 空值判断
来源：http://ac.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ga.huixiangedu.cn

[Q22] 排序
来源：http://yw.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bv.bjjhwx.cn

[Q23] 分页
来源：http://ci.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ch.szsharing.cn

[Q24] 去重
来源：http://td.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://bd.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://cz.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ql.huixiangedu.cn

[Q26] 计数
来源：http://mc.521024.cn

SELECT COUNT(*) FROM users;
来源：http://yw.chemitech.net.cn

[Q27] 条件计数
来源：http://td.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xr.hahajie.cn

[Q28] 求和与平均
来源：http://po.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nb.jctech888.com.cn

[Q29] 最大最小值
来源：http://ux.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zj.panjiajie.cn

[Q30] 分组统计
来源：http://gt.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tp.hnjuh.cn

[Q31] 分组后过滤
来源：http://tf.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fj.hahajie.cn

[Q32] 分组拼接字符串
来源：http://kx.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ly.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bd.huixinmuqiang.cn

[Q33] 多列分组
来源：http://pj.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ep.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ec.jianghongdianzi.cn

SELECT * FROM (
来源：http://zw.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pc.521024.cn

) t WHERE rn = 1;
来源：http://pe.nszjky.cn

[Q35] 内连接
来源：http://tx.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vl.szsharing.cn

[Q36] 左连接
来源：http://og.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wk.yuexingan06.cn

[Q37] 右连接
来源：http://hj.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cc.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wz.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://go.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://fz.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sf.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sb.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rn.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://es.lnxyls.cn

[Q41] 多表连接
来源：http://cf.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ph.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://bt.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://nl.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://jl.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://la.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://am.gzmigu.cn

[Q43] 标量子查询
来源：http://lj.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wo.chemitech.net.cn

[Q44] IN 子查询
来源：http://oi.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fr.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://xm.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ei.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xj.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wl.shtwfgs.cn

[Q47] 与平均值比较
来源：http://cs.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://af.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://mx.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fn.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ez.shxzukj.cn

[Q49] 更新单行
来源：http://ak.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rf.szsharing.cn

[Q50] 批量更新
来源：http://va.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zb.nszjky.cn

[Q51] 用子查询更新
来源：http://cr.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://be.gzmigu.cn

[Q52] 删除指定行
来源：http://zz.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://ag.gzmigu.cn

[Q53] 按条件删除
来源：http://va.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://so.huixinmuqiang.cn

[Q54] 清空表
来源：http://tm.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ug.huanxung.cn

[Q55] 排名（并列占位）
来源：http://un.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ae.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://gj.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hg.nszjky.cn

[Q57] 行号
来源：http://ti.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ht.jctech888.com.cn

[Q58] 累计求和
来源：http://lr.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ef.szxytkj.cn

[Q59] 分组内累计
来源：http://rq.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ca.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://lp.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tl.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://em.shxzukj.cn

[Q61] 移动平均
来源：http://wh.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pd.bjjhwx.cn

[Q62] 分组占比
来源：http://bx.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ud.bjjhwx.cn

[Q63] 开启事务
来源：http://id.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rh.bookmarksfly.cn

[Q64] 提交事务
来源：http://vv.asd995.cn

COMMIT;
来源：http://hb.newstarts.cn

[Q65] 回滚事务
来源：http://rc.nicolike.cn

ROLLBACK;
来源：http://tu.lnxyls.cn

[Q66] 行锁查询
来源：http://kv.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xl.shtwfgs.cn


<!-- 参考信息 -->