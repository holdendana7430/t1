代发 wailian999

PHP:  // 手写递归函数
来源：http://yf.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tl.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sr.shtwfgs.cn

Java: // 手写递归
来源：http://sk.huanxung.cn

Go:   // 手写递归
来源：http://ic.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ro.yuexingan06.cn

C#:   // 手写递归
来源：http://qi.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gz.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://it.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ki.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://js.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xc.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vq.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ql.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cv.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ss.shtwfgs.cn

================================================================================
来源：http://yl.yuntaijiaju.cn

O. 并发与异步
来源：http://ln.jctech888.com.cn

================================================================================
来源：http://lc.nicolike.cn

[O01] 启动一个线程
来源：http://bs.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kx.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sj.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lg.asd995.cn

TS:   // 同 JS
来源：http://qw.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://uz.newstarts.cn

Go:   go f()
来源：http://js.colortex.cn

Ruby: Thread.new { f }
来源：http://cg.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ou.colortex.cn

[O02] 使用线程池
来源：http://hm.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ls.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cs.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://mi.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://tr.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fq.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://df.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nw.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mm.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://hh.huanxung.cn

Py:   with lock: shared += 1
来源：http://tm.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://cy.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tl.521024.cn

TS:   // 同 JS
来源：http://ok.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://oo.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cf.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ez.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://uc.521024.cn

[O04] 定义异步函数并等待
来源：http://df.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://wc.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ky.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://th.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ko.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ro.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mb.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://li.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://gq.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://of.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://li.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wn.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://hy.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://wh.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yl.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fb.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://vl.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nr.huanxung.cn

[O06] 使用进程池
来源：http://mm.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sp.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pe.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://cl.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://yy.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fy.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bj.nicolike.cn

Ruby: // fork 块
来源：http://or.szxytkj.cn

C#:   Parallel.For
来源：http://eh.bookmarksfly.cn

================================================================================
来源：http://we.bookmarksfly.cn

P. 常用工具函数
来源：http://wt.shtwfgs.cn

================================================================================
来源：http://le.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://dx.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://ei.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hy.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ka.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://jv.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://vv.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://ht.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://kg.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://fo.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://xx.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oq.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://td.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mt.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lh.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://za.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://im.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ki.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ki.shxzukj.cn

[P03] 生成短随机字符串
来源：http://kf.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vw.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oy.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yk.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cm.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://at.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dv.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mi.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gl.shxzukj.cn

[P04] 求长度
来源：http://ap.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jy.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ng.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hu.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kp.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://lm.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://yw.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://ai.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://va.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://be.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rq.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tt.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vv.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pg.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mk.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xo.hahajie.cn

Ruby: a == b
来源：http://rv.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ho.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yw.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hw.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://uj.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pa.nszjky.cn

TS:   if (x == null) {}
来源：http://qg.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tp.hnjuh.cn

Go:   if x == nil {}
来源：http://nz.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zn.shxzskj.cn

C#:   if (x is null) {}
来源：http://af.gzmigu.cn

[P07] 防抖与节流
来源：http://yp.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zy.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://dm.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pd.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nq.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wo.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xz.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fv.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cp.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://ik.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lc.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xu.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gp.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jc.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zg.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bj.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://po.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fe.yuntaijiaju.cn

================================================================================
来源：http://zm.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hx.gzmigu.cn

================================================================================
来源：http://me.haigaiapp.cn

[Q01] 创建表
来源：http://hm.bjjhwx.cn

CREATE TABLE users (
来源：http://aq.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xo.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://tc.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ws.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yz.huixinmuqiang.cn

);
来源：http://nf.huanxung.cn

[Q02] 创建带外键的表
来源：http://sx.shxzukj.cn

CREATE TABLE orders (
来源：http://to.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gw.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://rk.nszjky.cn

amount DECIMAL(10, 2),
来源：http://oe.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jx.521024.cn

);
来源：http://xw.lnxyls.cn

[Q03] 增加列
来源：http://gc.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ru.shxzskj.cn

[Q04] 修改列类型
来源：http://xt.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dh.shxzukj.cn

[Q05] 重命名列
来源：http://rk.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oz.nszjky.cn

[Q06] 删除列
来源：http://bj.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://se.nicolike.cn

[Q07] 删除表
来源：http://ua.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://pg.szxytkj.cn

[Q08] 创建普通索引
来源：http://xv.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yb.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://hp.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fw.yuntaijiaju.cn

[Q10] 插入单行
来源：http://gp.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ed.shxzskj.cn

[Q11] 一次插入多行
来源：http://he.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ci.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://ql.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ek.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://it.hnjuh.cn

[Q13] 忽略重复插入
来源：http://tm.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mi.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://je.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sr.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gl.huanxung.cn

[Q15] 查询全部
来源：http://kk.bookmarksfly.cn

SELECT * FROM users;
来源：http://hz.nszjky.cn

[Q16] 查询指定列
来源：http://dk.newstarts.cn

SELECT id, name FROM users;
来源：http://ll.nicolike.cn

[Q17] 条件查询
来源：http://nm.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gq.jctech888.com.cn

[Q18] 模糊匹配
来源：http://yg.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hg.bookmarksfly.cn

[Q19] 范围查询
来源：http://pp.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ol.hahajie.cn

[Q20] IN 列表
来源：http://zf.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kd.jianghongdianzi.cn

[Q21] 空值判断
来源：http://lv.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qh.shxzukj.cn

[Q22] 排序
来源：http://uv.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bj.newstarts.cn

[Q23] 分页
来源：http://vq.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gq.shxzukj.cn

[Q24] 去重
来源：http://or.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://fv.9csxet.cn

[Q25] 只取前 N 条
来源：http://jf.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://li.huixinmuqiang.cn

[Q26] 计数
来源：http://ad.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://eh.shxzskj.cn

[Q27] 条件计数
来源：http://lr.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uq.haigaiapp.cn

[Q28] 求和与平均
来源：http://fj.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zf.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://bu.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://is.szsharing.cn

[Q30] 分组统计
来源：http://yc.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://al.521024.cn

[Q31] 分组后过滤
来源：http://nq.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sj.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://tx.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ox.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iv.bookmarksfly.cn

[Q33] 多列分组
来源：http://ez.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ud.asd995.cn

[Q34] 每组取第一条
来源：http://zo.wgjwhj.cn

SELECT * FROM (
来源：http://rc.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ms.wgjwhj.cn

) t WHERE rn = 1;
来源：http://jv.asd995.cn

[Q35] 内连接
来源：http://bu.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fp.muxihuayi.cn

[Q36] 左连接
来源：http://yj.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ck.nicolike.cn

[Q37] 右连接
来源：http://so.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ny.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vv.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kl.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://ot.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sd.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ax.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aq.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ga.huixinmuqiang.cn

[Q41] 多表连接
来源：http://mf.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bi.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://fp.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://mk.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://pt.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://tb.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ju.wgjwhj.cn

[Q43] 标量子查询
来源：http://lm.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sz.shxzukj.cn

[Q44] IN 子查询
来源：http://zq.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fn.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://ls.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hs.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://de.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bp.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ck.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mf.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://jv.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mv.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://sc.9csxet.cn

[Q49] 更新单行
来源：http://lx.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fd.wgjwhj.cn

[Q50] 批量更新
来源：http://me.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jk.wgjwhj.cn

[Q51] 用子查询更新
来源：http://xc.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xn.haigaiapp.cn

[Q52] 删除指定行
来源：http://pg.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://es.shxzskj.cn

[Q53] 按条件删除
来源：http://lh.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ej.panjiajie.cn

[Q54] 清空表
来源：http://od.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://gf.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://hi.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://us.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://cd.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ko.wgjwhj.cn

[Q57] 行号
来源：http://bn.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wb.521024.cn

[Q58] 累计求和
来源：http://he.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ed.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://wj.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zt.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://vb.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dr.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://by.jianghongdianzi.cn

[Q61] 移动平均
来源：http://sc.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://an.haigaiapp.cn

[Q62] 分组占比
来源：http://fx.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://to.muxihuayi.cn

[Q63] 开启事务
来源：http://md.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zc.shxzskj.cn

[Q64] 提交事务
来源：http://nt.haigaiapp.cn

COMMIT;
来源：http://ji.chemitech.net.cn


<!-- 参考信息 -->