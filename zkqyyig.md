代发 wailian999

Go:   // 手写递归
来源：http://jz.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vc.nicolike.cn

C#:   // 手写递归
来源：http://yg.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kq.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ge.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kd.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gg.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rb.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rg.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jc.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fl.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zd.shxzukj.cn

================================================================================
来源：http://cf.nszjky.cn

O. 并发与异步
来源：http://gs.lnxyls.cn

================================================================================
来源：http://yb.jctech888.com.cn

[O01] 启动一个线程
来源：http://rb.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tb.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fn.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vq.shxzskj.cn

TS:   // 同 JS
来源：http://zp.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://ri.asd995.cn

Go:   go f()
来源：http://af.szsharing.cn

Ruby: Thread.new { f }
来源：http://em.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://se.jianghongdianzi.cn

[O02] 使用线程池
来源：http://sa.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nn.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cq.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://hm.nicolike.cn

TS:   // worker_threads 线程池
来源：http://we.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wp.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hw.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kz.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ga.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://xh.521024.cn

Py:   with lock: shared += 1
来源：http://va.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://gg.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cr.szxytkj.cn

TS:   // 同 JS
来源：http://zj.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://dk.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://po.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wk.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://dj.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://os.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://sa.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yk.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://qt.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lb.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fq.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pw.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vg.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://bp.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://ym.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://hc.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lu.colortex.cn

JS:   await Promise.all(tasks)
来源：http://ht.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://mg.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lo.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zt.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ke.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dj.wgjwhj.cn

[O06] 使用进程池
来源：http://xd.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rc.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ey.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://yo.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://ks.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oi.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yt.huixinmuqiang.cn

Ruby: // fork 块
来源：http://uk.chemitech.net.cn

C#:   Parallel.For
来源：http://fa.lnxyls.cn

================================================================================
来源：http://eb.hnjuh.cn

P. 常用工具函数
来源：http://qp.asd995.cn

================================================================================
来源：http://yn.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://qe.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://pq.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zm.szsharing.cn

JS:   crypto.randomUUID()
来源：http://wk.521024.cn

TS:   crypto.randomUUID()
来源：http://mz.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://ab.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://xl.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://dd.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://la.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://rw.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ca.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tg.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ao.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ty.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nf.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jr.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bv.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vh.hahajie.cn

[P03] 生成短随机字符串
来源：http://vp.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ls.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sf.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oc.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bz.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sv.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uu.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lg.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ng.colortex.cn

[P04] 求长度
来源：http://fe.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://va.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cy.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jt.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cu.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://jq.huanxung.cn

Go:   len(arr);  len(m)
来源：http://jz.nicolike.cn

Ruby: x.length;  x.size
来源：http://yr.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ts.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://mq.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pu.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ab.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ss.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ek.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zo.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qy.nszjky.cn

Ruby: a == b
来源：http://xc.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ok.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zo.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ca.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://pa.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lv.shxzukj.cn

TS:   if (x == null) {}
来源：http://yl.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://er.colortex.cn

Go:   if x == nil {}
来源：http://tg.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kf.521024.cn

C#:   if (x is null) {}
来源：http://oy.huixiangedu.cn

[P07] 防抖与节流
来源：http://ku.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://od.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://np.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ix.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tz.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pj.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mv.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gf.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hj.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://pv.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eg.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cq.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fp.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xw.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://te.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dk.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ta.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hj.nszjky.cn

================================================================================
来源：http://ov.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ld.nicolike.cn

================================================================================
来源：http://qi.shxzukj.cn

[Q01] 创建表
来源：http://uz.huixinmuqiang.cn

CREATE TABLE users (
来源：http://vr.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qn.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://zc.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://js.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gi.chemitech.net.cn

);
来源：http://kn.521024.cn

[Q02] 创建带外键的表
来源：http://qk.jctech888.com.cn

CREATE TABLE orders (
来源：http://bn.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ji.muxihuayi.cn

user_id INT NOT NULL,
来源：http://ts.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://gn.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rt.wgjwhj.cn

);
来源：http://gq.huanxung.cn

[Q03] 增加列
来源：http://gc.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fp.gzmigu.cn

[Q04] 修改列类型
来源：http://ox.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rn.shtwfgs.cn

[Q05] 重命名列
来源：http://eg.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jj.9csxet.cn

[Q06] 删除列
来源：http://mg.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qf.asd995.cn

[Q07] 删除表
来源：http://jk.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://uc.hnjuh.cn

[Q08] 创建普通索引
来源：http://ip.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lw.shxzukj.cn

[Q09] 创建唯一索引
来源：http://py.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yl.huanxung.cn

[Q10] 插入单行
来源：http://ke.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://me.haigaiapp.cn

[Q11] 一次插入多行
来源：http://jz.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xa.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://uw.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bk.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nn.szsharing.cn

[Q13] 忽略重复插入
来源：http://ah.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ib.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://vt.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zm.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ok.jctech888.com.cn

[Q15] 查询全部
来源：http://zb.nicolike.cn

SELECT * FROM users;
来源：http://kd.shxzskj.cn

[Q16] 查询指定列
来源：http://xa.szsharing.cn

SELECT id, name FROM users;
来源：http://sx.hnjuh.cn

[Q17] 条件查询
来源：http://sl.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://df.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://jl.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ev.9csxet.cn

[Q19] 范围查询
来源：http://zs.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hf.lnxyls.cn

[Q20] IN 列表
来源：http://bd.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mf.szxytkj.cn

[Q21] 空值判断
来源：http://ur.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://id.shxzukj.cn

[Q22] 排序
来源：http://un.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ex.9csxet.cn

[Q23] 分页
来源：http://jr.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lr.asd995.cn

[Q24] 去重
来源：http://sv.521024.cn

SELECT DISTINCT city FROM users;
来源：http://cc.hnjuh.cn

[Q25] 只取前 N 条
来源：http://bt.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cs.haigaiapp.cn

[Q26] 计数
来源：http://br.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://ju.yuexingan06.cn

[Q27] 条件计数
来源：http://tj.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ix.shxzukj.cn

[Q28] 求和与平均
来源：http://mn.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ob.colortex.cn

[Q29] 最大最小值
来源：http://ln.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tt.szsharing.cn

[Q30] 分组统计
来源：http://ir.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bx.panjiajie.cn

[Q31] 分组后过滤
来源：http://hu.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yc.huanxung.cn

[Q32] 分组拼接字符串
来源：http://fo.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pt.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pi.hnjuh.cn

[Q33] 多列分组
来源：http://ek.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ai.newstarts.cn

[Q34] 每组取第一条
来源：http://jp.shxzskj.cn

SELECT * FROM (
来源：http://ci.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://im.szsharing.cn

) t WHERE rn = 1;
来源：http://ux.yuntaijiaju.cn

[Q35] 内连接
来源：http://rp.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://we.muxihuayi.cn

[Q36] 左连接
来源：http://uf.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://au.shxzskj.cn

[Q37] 右连接
来源：http://qf.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yw.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ul.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://en.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://od.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ep.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hp.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jr.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pa.shxzskj.cn

[Q41] 多表连接
来源：http://uj.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ja.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://lp.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://zv.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://bl.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://vz.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nz.asd995.cn

[Q43] 标量子查询
来源：http://lm.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.newstarts.cn

[Q44] IN 子查询
来源：http://fu.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sw.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://vu.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gn.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://st.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nl.haigaiapp.cn

[Q47] 与平均值比较
来源：http://wz.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://hf.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ef.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://wf.panjiajie.cn

[Q49] 更新单行
来源：http://lb.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gd.hnjuh.cn

[Q50] 批量更新
来源：http://lp.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wg.chemitech.net.cn

[Q51] 用子查询更新
来源：http://il.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gz.jctech888.com.cn

[Q52] 删除指定行
来源：http://qk.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://zy.hnjuh.cn

[Q53] 按条件删除
来源：http://fe.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rw.bjjhwx.cn

[Q54] 清空表
来源：http://rp.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://vm.9csxet.cn

[Q55] 排名（并列占位）
来源：http://nu.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://am.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://tf.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ye.jianghongdianzi.cn

[Q57] 行号
来源：http://aw.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vy.nszjky.cn

[Q58] 累计求和
来源：http://yz.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kq.huanxung.cn

[Q59] 分组内累计
来源：http://sa.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://op.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://ya.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xt.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://il.wgjwhj.cn

[Q61] 移动平均
来源：http://tr.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vt.bookmarksfly.cn

[Q62] 分组占比
来源：http://vp.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iv.hnjuh.cn

[Q63] 开启事务
来源：http://mv.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dp.wgjwhj.cn

[Q64] 提交事务
来源：http://ox.asd995.cn

COMMIT;
来源：http://xk.bookmarksfly.cn

[Q65] 回滚事务
来源：http://ao.bjjhwx.cn

ROLLBACK;
来源：http://cj.huixiangedu.cn

[Q66] 行锁查询
来源：http://ls.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pg.yuntaijiaju.cn


<!-- 参考信息 -->