代发 wailian999

Go:   // 手写递归
来源：http://st.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wl.bookmarksfly.cn

C#:   // 手写递归
来源：http://wy.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cb.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fw.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pl.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lj.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rp.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ah.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sf.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hs.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fy.yuntaijiaju.cn

================================================================================
来源：http://hr.wgjwhj.cn

O. 并发与异步
来源：http://xy.muxihuayi.cn

================================================================================
来源：http://bi.hahajie.cn

[O01] 启动一个线程
来源：http://oa.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vh.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aa.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hg.huixiangedu.cn

TS:   // 同 JS
来源：http://ch.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://ws.newstarts.cn

Go:   go f()
来源：http://kl.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://jg.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://ys.panjiajie.cn

[O02] 使用线程池
来源：http://uq.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sq.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hv.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://mw.colortex.cn

TS:   // worker_threads 线程池
来源：http://di.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gc.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ih.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cq.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ne.nicolike.cn

[O03] 加锁保护共享数据
来源：http://ge.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://jo.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://ws.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sa.yuntaijiaju.cn

TS:   // 同 JS
来源：http://sn.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://uv.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ie.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fz.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://hk.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://mx.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://qn.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rb.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://rg.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hy.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yv.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wi.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://th.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://ys.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://js.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://gc.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yu.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://xe.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://pa.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cm.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lt.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://dm.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qo.yuntaijiaju.cn

[O06] 使用进程池
来源：http://zj.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xn.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aa.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://xu.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://vk.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rx.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lu.newstarts.cn

Ruby: // fork 块
来源：http://bn.haigaiapp.cn

C#:   Parallel.For
来源：http://ig.9csxet.cn

================================================================================
来源：http://fq.shxzukj.cn

P. 常用工具函数
来源：http://oz.jctech888.com.cn

================================================================================
来源：http://zx.haigaiapp.cn

[P01] 生成 UUID
来源：http://ns.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://tk.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xl.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://br.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://om.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://bn.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://nm.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://eg.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://nr.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://xi.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nd.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yx.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xw.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://et.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lf.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rz.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qz.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yc.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://wc.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tn.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://so.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rv.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bu.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sf.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xb.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fs.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yx.chemitech.net.cn

[P04] 求长度
来源：http://it.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qm.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nh.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vx.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zj.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://ll.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://pi.gzmigu.cn

Ruby: x.length;  x.size
来源：http://qd.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ry.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://zv.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sn.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ol.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ym.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ig.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wh.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bk.huixinmuqiang.cn

Ruby: a == b
来源：http://xq.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ws.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oh.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pk.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://fe.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://da.szsharing.cn

TS:   if (x == null) {}
来源：http://ir.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rg.wgjwhj.cn

Go:   if x == nil {}
来源：http://xp.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ie.521024.cn

C#:   if (x is null) {}
来源：http://cl.shxzskj.cn

[P07] 防抖与节流
来源：http://nf.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uz.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://ap.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ph.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pp.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://op.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mn.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ae.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bq.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://ci.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mr.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pe.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dj.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mo.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://an.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ld.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://au.shxzukj.cn

================================================================================
来源：http://vx.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gd.wgjwhj.cn

================================================================================
来源：http://bp.nicolike.cn

[Q01] 创建表
来源：http://lz.asd995.cn

CREATE TABLE users (
来源：http://fm.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yw.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://or.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://hj.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pa.colortex.cn

);
来源：http://cb.hnjuh.cn

[Q02] 创建带外键的表
来源：http://op.szxytkj.cn

CREATE TABLE orders (
来源：http://di.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cx.lnxyls.cn

user_id INT NOT NULL,
来源：http://sv.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://rl.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qw.wgjwhj.cn

);
来源：http://ek.nicolike.cn

[Q03] 增加列
来源：http://fu.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kc.shtwfgs.cn

[Q04] 修改列类型
来源：http://fg.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tz.wgjwhj.cn

[Q05] 重命名列
来源：http://ld.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mx.shxzukj.cn

[Q06] 删除列
来源：http://gj.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gj.newstarts.cn

[Q07] 删除表
来源：http://tw.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://cp.lnxyls.cn

[Q08] 创建普通索引
来源：http://qy.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jg.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://ly.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oj.bjjhwx.cn

[Q10] 插入单行
来源：http://fp.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vy.hnjuh.cn

[Q11] 一次插入多行
来源：http://fd.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cr.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://ao.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xb.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ci.szxytkj.cn

[Q13] 忽略重复插入
来源：http://pu.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yb.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://xs.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gr.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rd.bookmarksfly.cn

[Q15] 查询全部
来源：http://dd.hnjuh.cn

SELECT * FROM users;
来源：http://hb.bookmarksfly.cn

[Q16] 查询指定列
来源：http://vl.asd995.cn

SELECT id, name FROM users;
来源：http://zc.521024.cn

[Q17] 条件查询
来源：http://on.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xx.yuexingan06.cn

[Q18] 模糊匹配
来源：http://oa.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sy.wgjwhj.cn

[Q19] 范围查询
来源：http://lx.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dm.jctech888.com.cn

[Q20] IN 列表
来源：http://gh.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bh.yuntaijiaju.cn

[Q21] 空值判断
来源：http://km.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xo.nicolike.cn

[Q22] 排序
来源：http://ic.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nc.huixiangedu.cn

[Q23] 分页
来源：http://ok.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wt.haigaiapp.cn

[Q24] 去重
来源：http://sn.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://ao.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://qc.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ar.haigaiapp.cn

[Q26] 计数
来源：http://wj.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://pp.jctech888.com.cn

[Q27] 条件计数
来源：http://nl.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://us.gzmigu.cn

[Q28] 求和与平均
来源：http://ev.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://es.colortex.cn

[Q29] 最大最小值
来源：http://on.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ec.bookmarksfly.cn

[Q30] 分组统计
来源：http://bb.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ga.9csxet.cn

[Q31] 分组后过滤
来源：http://qa.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yj.nszjky.cn

[Q32] 分组拼接字符串
来源：http://gi.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qh.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://er.lnxyls.cn

[Q33] 多列分组
来源：http://tj.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ld.shxzukj.cn

[Q34] 每组取第一条
来源：http://on.yuexingan06.cn

SELECT * FROM (
来源：http://oi.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lf.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://xh.muxihuayi.cn

[Q35] 内连接
来源：http://kw.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ky.nszjky.cn

[Q36] 左连接
来源：http://gl.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bb.newstarts.cn

[Q37] 右连接
来源：http://rh.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kd.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ru.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bb.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://uh.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ny.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iy.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jg.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aw.9csxet.cn

[Q41] 多表连接
来源：http://ix.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mw.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://au.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ao.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://gz.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://dp.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://al.szsharing.cn

[Q43] 标量子查询
来源：http://rb.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xm.bookmarksfly.cn

[Q44] IN 子查询
来源：http://nf.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ct.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://ew.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ny.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gm.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://du.asd995.cn

[Q47] 与平均值比较
来源：http://qk.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kr.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://fx.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://un.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://nk.szsharing.cn

[Q49] 更新单行
来源：http://kp.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ga.wgjwhj.cn

[Q50] 批量更新
来源：http://rk.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mn.szxytkj.cn

[Q51] 用子查询更新
来源：http://xm.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://au.yuexingan06.cn

[Q52] 删除指定行
来源：http://kz.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://jx.shxzskj.cn

[Q53] 按条件删除
来源：http://jx.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ef.asd995.cn

[Q54] 清空表
来源：http://mb.9csxet.cn

TRUNCATE TABLE logs;
来源：http://hl.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://cu.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://li.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://tz.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jf.jctech888.com.cn

[Q57] 行号
来源：http://fy.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wi.huanxung.cn

[Q58] 累计求和
来源：http://hb.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gb.colortex.cn

[Q59] 分组内累计
来源：http://hr.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sa.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://wh.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ux.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cr.wgjwhj.cn

[Q61] 移动平均
来源：http://xn.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rs.huixinmuqiang.cn

[Q62] 分组占比
来源：http://ze.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xx.hnjuh.cn

[Q63] 开启事务
来源：http://cq.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eh.huixinmuqiang.cn

[Q64] 提交事务
来源：http://jl.gzmigu.cn

COMMIT;
来源：http://ea.yuexingan06.cn

[Q65] 回滚事务
来源：http://wf.huixinmuqiang.cn

ROLLBACK;
来源：http://jw.hahajie.cn

[Q66] 行锁查询
来源：http://yk.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cg.szxytkj.cn


<!-- 参考信息 -->