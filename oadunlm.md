代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://do.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pt.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jx.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ty.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iw.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xo.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://is.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://th.wgjwhj.cn

================================================================================
来源：http://jg.huixinmuqiang.cn

O. 并发与异步
来源：http://fb.haigaiapp.cn

================================================================================
来源：http://de.521024.cn

[O01] 启动一个线程
来源：http://ln.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jm.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ym.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tu.9csxet.cn

TS:   // 同 JS
来源：http://uk.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://ht.bjjhwx.cn

Go:   go f()
来源：http://zx.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://fs.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://rn.chemitech.net.cn

[O02] 使用线程池
来源：http://fd.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://am.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lp.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://qs.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://nx.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://af.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tl.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ul.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ar.nicolike.cn

[O03] 加锁保护共享数据
来源：http://nw.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://iq.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://cs.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://it.hnjuh.cn

TS:   // 同 JS
来源：http://da.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://el.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jv.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fh.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://qq.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://ma.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://gw.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://of.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://pa.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oy.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ch.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rx.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qq.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://hh.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://bx.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://oi.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vr.asd995.cn

JS:   await Promise.all(tasks)
来源：http://ly.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://ki.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uh.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hg.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ik.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wo.bookmarksfly.cn

[O06] 使用进程池
来源：http://yr.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ti.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wd.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://wn.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://jk.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yr.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xx.lnxyls.cn

Ruby: // fork 块
来源：http://zg.huixinmuqiang.cn

C#:   Parallel.For
来源：http://pk.yuexingan06.cn

================================================================================
来源：http://xi.colortex.cn

P. 常用工具函数
来源：http://to.521024.cn

================================================================================
来源：http://oe.hahajie.cn

[P01] 生成 UUID
来源：http://nu.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://vy.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eq.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://yd.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://ww.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://yt.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://pw.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://hx.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://ic.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://jj.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sx.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vb.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nm.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lq.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pv.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hn.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fj.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pn.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://fi.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jp.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ik.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tt.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hx.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rt.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bt.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zr.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jd.colortex.cn

[P04] 求长度
来源：http://bg.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://to.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bv.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gy.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pf.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://nm.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://rn.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://qi.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dp.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://er.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mh.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ew.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ta.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cz.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jb.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ck.szxytkj.cn

Ruby: a == b
来源：http://qb.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lj.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yg.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rd.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://rm.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hx.shxzukj.cn

TS:   if (x == null) {}
来源：http://td.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jj.shxzskj.cn

Go:   if x == nil {}
来源：http://us.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sy.asd995.cn

C#:   if (x is null) {}
来源：http://fv.wgjwhj.cn

[P07] 防抖与节流
来源：http://kw.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zq.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://ht.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cn.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tm.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qs.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ze.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pa.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ck.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://wn.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hx.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ss.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pc.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://my.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ro.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kq.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ih.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://na.bookmarksfly.cn

================================================================================
来源：http://ux.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fj.asd995.cn

================================================================================
来源：http://rm.chemitech.net.cn

[Q01] 创建表
来源：http://lf.huanxung.cn

CREATE TABLE users (
来源：http://ka.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sq.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://qz.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://ca.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wk.asd995.cn

);
来源：http://ut.hahajie.cn

[Q02] 创建带外键的表
来源：http://rb.shxzskj.cn

CREATE TABLE orders (
来源：http://io.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ql.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://ec.colortex.cn

amount DECIMAL(10, 2),
来源：http://wx.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pj.9csxet.cn

);
来源：http://lz.hnjuh.cn

[Q03] 增加列
来源：http://ns.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vm.bookmarksfly.cn

[Q04] 修改列类型
来源：http://oc.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hp.shxzskj.cn

[Q05] 重命名列
来源：http://yy.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zf.521024.cn

[Q06] 删除列
来源：http://gb.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qu.haigaiapp.cn

[Q07] 删除表
来源：http://em.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://gv.bjjhwx.cn

[Q08] 创建普通索引
来源：http://cb.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ts.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://tg.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jn.nicolike.cn

[Q10] 插入单行
来源：http://bj.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dw.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://zf.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xl.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://fg.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tk.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tw.nszjky.cn

[Q13] 忽略重复插入
来源：http://ge.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gk.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://ja.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jm.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ut.bjjhwx.cn

[Q15] 查询全部
来源：http://np.nszjky.cn

SELECT * FROM users;
来源：http://np.szxytkj.cn

[Q16] 查询指定列
来源：http://ud.yuexingan06.cn

SELECT id, name FROM users;
来源：http://fx.newstarts.cn

[Q17] 条件查询
来源：http://uk.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://te.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://og.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yo.muxihuayi.cn

[Q19] 范围查询
来源：http://am.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wv.gzmigu.cn

[Q20] IN 列表
来源：http://cn.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://az.huanxung.cn

[Q21] 空值判断
来源：http://vq.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ww.haigaiapp.cn

[Q22] 排序
来源：http://fg.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rf.panjiajie.cn

[Q23] 分页
来源：http://eu.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://de.shxzukj.cn

[Q24] 去重
来源：http://ef.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://bh.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://de.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bg.nszjky.cn

[Q26] 计数
来源：http://hx.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://od.nicolike.cn

[Q27] 条件计数
来源：http://zt.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hi.hnjuh.cn

[Q28] 求和与平均
来源：http://ec.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kv.huixiangedu.cn

[Q29] 最大最小值
来源：http://jm.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sj.nszjky.cn

[Q30] 分组统计
来源：http://cx.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ii.lnxyls.cn

[Q31] 分组后过滤
来源：http://rd.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://az.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://rj.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aq.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pp.9csxet.cn

[Q33] 多列分组
来源：http://po.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://do.nszjky.cn

[Q34] 每组取第一条
来源：http://ux.szsharing.cn

SELECT * FROM (
来源：http://mw.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hu.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://wv.newstarts.cn

[Q35] 内连接
来源：http://xz.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cy.chemitech.net.cn

[Q36] 左连接
来源：http://ng.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gr.szsharing.cn

[Q37] 右连接
来源：http://pf.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nc.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://za.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://de.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://sv.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vg.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://my.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xq.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://md.jctech888.com.cn

[Q41] 多表连接
来源：http://jj.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ar.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://xr.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://mv.asd995.cn

[Q42] 连接条件附加过滤
来源：http://dz.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://is.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hw.chemitech.net.cn

[Q43] 标量子查询
来源：http://pz.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zg.521024.cn

[Q44] IN 子查询
来源：http://ao.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qk.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://rl.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tq.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tw.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rd.bjjhwx.cn

[Q47] 与平均值比较
来源：http://jj.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nb.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://dy.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://my.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://wq.huixinmuqiang.cn

[Q49] 更新单行
来源：http://hw.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uf.huixiangedu.cn

[Q50] 批量更新
来源：http://sr.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vl.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://if.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hk.panjiajie.cn

[Q52] 删除指定行
来源：http://xz.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://vs.521024.cn

[Q53] 按条件删除
来源：http://ix.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qq.huixiangedu.cn

[Q54] 清空表
来源：http://mh.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://dr.521024.cn

[Q55] 排名（并列占位）
来源：http://kn.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vo.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://wk.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jd.hnjuh.cn

[Q57] 行号
来源：http://at.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rd.bookmarksfly.cn

[Q58] 累计求和
来源：http://pc.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cy.hnjuh.cn

[Q59] 分组内累计
来源：http://sq.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rh.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://cs.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ph.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mr.newstarts.cn

[Q61] 移动平均
来源：http://ia.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mz.newstarts.cn

[Q62] 分组占比
来源：http://jq.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ce.lnxyls.cn

[Q63] 开启事务
来源：http://fx.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ye.huixinmuqiang.cn

[Q64] 提交事务
来源：http://gy.hahajie.cn

COMMIT;
来源：http://zo.haigaiapp.cn

[Q65] 回滚事务
来源：http://ud.nszjky.cn

ROLLBACK;
来源：http://el.shxzskj.cn

[Q66] 行锁查询
来源：http://fo.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mh.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://dj.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xs.bjjhwx.cn

[Q68] 保存点
来源：http://rt.shxzukj.cn

SAVEPOINT sp1;
来源：http://qx.yuexingan06.cn


<!-- 参考信息 -->