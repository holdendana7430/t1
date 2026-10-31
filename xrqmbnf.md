代发 wailian999

Go:   // 手写递归
来源：http://uv.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uo.jianghongdianzi.cn

C#:   // 手写递归
来源：http://gv.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oe.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://go.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ir.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mj.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mo.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gk.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://is.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://we.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ar.9csxet.cn

================================================================================
来源：http://ys.szsharing.cn

O. 并发与异步
来源：http://ne.yuntaijiaju.cn

================================================================================
来源：http://op.nszjky.cn

[O01] 启动一个线程
来源：http://pg.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://na.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ly.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dq.nszjky.cn

TS:   // 同 JS
来源：http://ka.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://de.szsharing.cn

Go:   go f()
来源：http://mj.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://kv.szsharing.cn

C#:   Task.Run(() => F());
来源：http://hy.yuntaijiaju.cn

[O02] 使用线程池
来源：http://dl.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jj.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tk.nszjky.cn

JS:   // worker_threads 线程池
来源：http://gr.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://uh.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wp.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://je.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sh.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sn.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://ji.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://os.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://iw.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mt.huanxung.cn

TS:   // 同 JS
来源：http://zx.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://fs.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jz.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://db.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://gd.nszjky.cn

[O04] 定义异步函数并等待
来源：http://ed.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://jx.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dx.hahajie.cn

JS:   async function f() { await g(); }
来源：http://xw.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://co.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ut.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qi.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hk.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://za.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://kh.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://kq.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://py.colortex.cn

JS:   await Promise.all(tasks)
来源：http://mh.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://rd.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jw.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ai.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://dq.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yz.bookmarksfly.cn

[O06] 使用进程池
来源：http://dg.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xd.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lo.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://kt.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://wu.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cw.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zt.shtwfgs.cn

Ruby: // fork 块
来源：http://ch.shxzskj.cn

C#:   Parallel.For
来源：http://qb.szsharing.cn

================================================================================
来源：http://xp.bookmarksfly.cn

P. 常用工具函数
来源：http://dr.jianghongdianzi.cn

================================================================================
来源：http://fa.szsharing.cn

[P01] 生成 UUID
来源：http://dp.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ei.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ru.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://kc.nszjky.cn

TS:   crypto.randomUUID()
来源：http://vl.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://wt.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://cb.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://rl.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://bc.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://iz.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mt.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cy.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wm.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bj.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://za.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pg.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pw.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cr.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://ix.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cm.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://im.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vb.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iv.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pi.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bs.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jc.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ki.asd995.cn

[P04] 求长度
来源：http://lb.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bi.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rm.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pi.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kb.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://wj.colortex.cn

Go:   len(arr);  len(m)
来源：http://yi.9csxet.cn

Ruby: x.length;  x.size
来源：http://qu.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ap.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://mu.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ll.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rn.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pz.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://va.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ye.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ve.jctech888.com.cn

Ruby: a == b
来源：http://ni.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tp.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xq.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yt.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://jb.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rv.huanxung.cn

TS:   if (x == null) {}
来源：http://jk.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xk.asd995.cn

Go:   if x == nil {}
来源：http://wn.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tz.chemitech.net.cn

C#:   if (x is null) {}
来源：http://kd.newstarts.cn

[P07] 防抖与节流
来源：http://rw.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://on.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://qr.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ch.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cp.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pg.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://at.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sr.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tz.nicolike.cn

[P08] 处理浮点精度问题
来源：http://px.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yv.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vn.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ah.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gu.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zo.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qj.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vb.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ja.huixinmuqiang.cn

================================================================================
来源：http://xf.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qp.haigaiapp.cn

================================================================================
来源：http://om.521024.cn

[Q01] 创建表
来源：http://gz.huixinmuqiang.cn

CREATE TABLE users (
来源：http://rb.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kh.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://yq.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://xp.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vb.panjiajie.cn

);
来源：http://gu.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://zm.bjjhwx.cn

CREATE TABLE orders (
来源：http://rb.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qc.panjiajie.cn

user_id INT NOT NULL,
来源：http://gj.nszjky.cn

amount DECIMAL(10, 2),
来源：http://hi.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zj.nicolike.cn

);
来源：http://br.jianghongdianzi.cn

[Q03] 增加列
来源：http://kn.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fx.haigaiapp.cn

[Q04] 修改列类型
来源：http://tt.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://so.haigaiapp.cn

[Q05] 重命名列
来源：http://mr.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ww.muxihuayi.cn

[Q06] 删除列
来源：http://be.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sx.shxzukj.cn

[Q07] 删除表
来源：http://xq.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://qp.wgjwhj.cn

[Q08] 创建普通索引
来源：http://tb.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zl.nszjky.cn

[Q09] 创建唯一索引
来源：http://dj.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tu.huixinmuqiang.cn

[Q10] 插入单行
来源：http://jw.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xm.asd995.cn

[Q11] 一次插入多行
来源：http://iu.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://na.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://al.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lx.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ge.panjiajie.cn

[Q13] 忽略重复插入
来源：http://mr.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ae.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://os.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oo.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://es.521024.cn

[Q15] 查询全部
来源：http://hi.bjjhwx.cn

SELECT * FROM users;
来源：http://jd.nszjky.cn

[Q16] 查询指定列
来源：http://ym.hnjuh.cn

SELECT id, name FROM users;
来源：http://iv.panjiajie.cn

[Q17] 条件查询
来源：http://vs.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wc.gzmigu.cn

[Q18] 模糊匹配
来源：http://ak.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wy.yuntaijiaju.cn

[Q19] 范围查询
来源：http://mt.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kh.nicolike.cn

[Q20] IN 列表
来源：http://kh.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qt.bjjhwx.cn

[Q21] 空值判断
来源：http://bl.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cl.chemitech.net.cn

[Q22] 排序
来源：http://sx.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fh.yuexingan06.cn

[Q23] 分页
来源：http://mr.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://su.huixiangedu.cn

[Q24] 去重
来源：http://gq.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://xn.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://ug.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kn.gzmigu.cn

[Q26] 计数
来源：http://jt.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://cv.asd995.cn

[Q27] 条件计数
来源：http://cn.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nu.521024.cn

[Q28] 求和与平均
来源：http://oe.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bq.hnjuh.cn

[Q29] 最大最小值
来源：http://fm.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zo.huixiangedu.cn

[Q30] 分组统计
来源：http://ul.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://or.colortex.cn

[Q31] 分组后过滤
来源：http://xp.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jy.colortex.cn

[Q32] 分组拼接字符串
来源：http://jr.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nt.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hc.huixiangedu.cn

[Q33] 多列分组
来源：http://ve.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lu.colortex.cn

[Q34] 每组取第一条
来源：http://px.huanxung.cn

SELECT * FROM (
来源：http://xu.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vn.asd995.cn

) t WHERE rn = 1;
来源：http://ft.gzmigu.cn

[Q35] 内连接
来源：http://hw.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ox.yuntaijiaju.cn

[Q36] 左连接
来源：http://bo.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ir.bookmarksfly.cn

[Q37] 右连接
来源：http://zb.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lw.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rc.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fl.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://co.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zb.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jw.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://po.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ql.newstarts.cn

[Q41] 多表连接
来源：http://tn.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xb.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://qx.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://mc.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://vp.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://gb.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xm.bookmarksfly.cn

[Q43] 标量子查询
来源：http://zq.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xr.shxzukj.cn

[Q44] IN 子查询
来源：http://gk.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://an.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://qc.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zt.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fc.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kr.hahajie.cn

[Q47] 与平均值比较
来源：http://lo.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://af.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://mw.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rb.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://ei.jctech888.com.cn

[Q49] 更新单行
来源：http://tp.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bx.szsharing.cn

[Q50] 批量更新
来源：http://sz.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yd.9csxet.cn

[Q51] 用子查询更新
来源：http://fw.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hl.bookmarksfly.cn

[Q52] 删除指定行
来源：http://ml.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://tr.newstarts.cn

[Q53] 按条件删除
来源：http://qe.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gt.yuntaijiaju.cn

[Q54] 清空表
来源：http://ky.nicolike.cn

TRUNCATE TABLE logs;
来源：http://bo.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://fe.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oc.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://xe.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://at.shxzskj.cn

[Q57] 行号
来源：http://dr.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hh.shxzukj.cn

[Q58] 累计求和
来源：http://op.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ej.asd995.cn

[Q59] 分组内累计
来源：http://wb.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zu.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://hd.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://af.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ez.shxzskj.cn

[Q61] 移动平均
来源：http://io.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wx.nicolike.cn

[Q62] 分组占比
来源：http://ch.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cq.chemitech.net.cn

[Q63] 开启事务
来源：http://ba.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tx.bookmarksfly.cn

[Q64] 提交事务
来源：http://yn.muxihuayi.cn

COMMIT;
来源：http://iv.panjiajie.cn

[Q65] 回滚事务
来源：http://ow.gzmigu.cn

ROLLBACK;
来源：http://qz.shtwfgs.cn

[Q66] 行锁查询
来源：http://bn.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ny.shxzukj.cn


<!-- 参考信息 -->