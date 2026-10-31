代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://st.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://do.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ny.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yv.shtwfgs.cn

================================================================================
来源：http://lj.shxzskj.cn

O. 并发与异步
来源：http://hu.colortex.cn

================================================================================
来源：http://yc.szxytkj.cn

[O01] 启动一个线程
来源：http://ye.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://df.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tu.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zo.huixinmuqiang.cn

TS:   // 同 JS
来源：http://cw.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://ar.hnjuh.cn

Go:   go f()
来源：http://uj.newstarts.cn

Ruby: Thread.new { f }
来源：http://rs.szsharing.cn

C#:   Task.Run(() => F());
来源：http://zz.nicolike.cn

[O02] 使用线程池
来源：http://dl.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sv.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ru.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://fx.hahajie.cn

TS:   // worker_threads 线程池
来源：http://uo.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ln.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kl.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ai.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://do.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://tn.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://yt.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://rz.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wr.szxytkj.cn

TS:   // 同 JS
来源：http://sn.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://sl.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hd.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oy.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://ci.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://zh.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://bw.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ta.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://nc.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fm.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qc.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vi.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oa.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://wp.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://nb.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://ed.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oo.colortex.cn

JS:   await Promise.all(tasks)
来源：http://sc.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://vv.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qm.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://en.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://ni.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://si.shxzukj.cn

[O06] 使用进程池
来源：http://ck.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gd.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zn.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://vp.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://uz.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ba.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bl.shtwfgs.cn

Ruby: // fork 块
来源：http://bk.huanxung.cn

C#:   Parallel.For
来源：http://ry.jctech888.com.cn

================================================================================
来源：http://ui.hahajie.cn

P. 常用工具函数
来源：http://wi.yuntaijiaju.cn

================================================================================
来源：http://tr.gzmigu.cn

[P01] 生成 UUID
来源：http://ys.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://kn.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://et.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://kj.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://zs.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://ol.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://xa.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ns.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://cy.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://hk.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cn.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nz.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lb.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zn.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wg.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ho.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ol.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://of.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://vb.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jx.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sf.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oc.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wg.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qd.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kl.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lz.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ja.yuexingan06.cn

[P04] 求长度
来源：http://ks.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zs.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fn.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://we.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yz.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://mi.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://qp.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ue.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pg.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://ji.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://je.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://li.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fz.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xn.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vp.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://px.panjiajie.cn

Ruby: a == b
来源：http://fj.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gg.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ki.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ly.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://dh.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rj.jctech888.com.cn

TS:   if (x == null) {}
来源：http://ry.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bx.huixiangedu.cn

Go:   if x == nil {}
来源：http://os.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://my.panjiajie.cn

C#:   if (x is null) {}
来源：http://ed.shxzskj.cn

[P07] 防抖与节流
来源：http://tb.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eg.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://yu.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xi.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gs.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xd.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bz.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oj.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bm.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://ws.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://km.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pm.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ya.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mv.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lv.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cn.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jq.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://os.chemitech.net.cn

================================================================================
来源：http://dq.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ep.colortex.cn

================================================================================
来源：http://do.bookmarksfly.cn

[Q01] 创建表
来源：http://bt.shxzskj.cn

CREATE TABLE users (
来源：http://mr.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kk.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://xt.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://oh.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qz.9csxet.cn

);
来源：http://nm.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://an.gzmigu.cn

CREATE TABLE orders (
来源：http://rr.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xy.gzmigu.cn

user_id INT NOT NULL,
来源：http://gx.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://ul.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sz.nicolike.cn

);
来源：http://mg.jianghongdianzi.cn

[Q03] 增加列
来源：http://xj.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yk.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://aj.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ah.chemitech.net.cn

[Q05] 重命名列
来源：http://bi.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ux.szxytkj.cn

[Q06] 删除列
来源：http://an.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bg.huixinmuqiang.cn

[Q07] 删除表
来源：http://rr.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://eh.muxihuayi.cn

[Q08] 创建普通索引
来源：http://zj.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zz.521024.cn

[Q09] 创建唯一索引
来源：http://tp.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ez.shxzukj.cn

[Q10] 插入单行
来源：http://jq.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uh.yuexingan06.cn

[Q11] 一次插入多行
来源：http://mf.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://os.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://xd.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zq.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bm.panjiajie.cn

[Q13] 忽略重复插入
来源：http://xh.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wc.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://jx.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mn.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dt.szsharing.cn

[Q15] 查询全部
来源：http://kz.szsharing.cn

SELECT * FROM users;
来源：http://ty.asd995.cn

[Q16] 查询指定列
来源：http://jj.chemitech.net.cn

SELECT id, name FROM users;
来源：http://zk.yuntaijiaju.cn

[Q17] 条件查询
来源：http://uy.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hb.szxytkj.cn

[Q18] 模糊匹配
来源：http://vl.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uz.chemitech.net.cn

[Q19] 范围查询
来源：http://bc.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gh.huixiangedu.cn

[Q20] IN 列表
来源：http://aq.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yr.nicolike.cn

[Q21] 空值判断
来源：http://tk.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uz.muxihuayi.cn

[Q22] 排序
来源：http://vm.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ok.hnjuh.cn

[Q23] 分页
来源：http://ae.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iu.521024.cn

[Q24] 去重
来源：http://ea.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://kf.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://px.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wp.shtwfgs.cn

[Q26] 计数
来源：http://oi.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://qz.nicolike.cn

[Q27] 条件计数
来源：http://kn.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mq.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://vt.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ww.wgjwhj.cn

[Q29] 最大最小值
来源：http://op.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jv.huanxung.cn

[Q30] 分组统计
来源：http://zm.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wp.chemitech.net.cn

[Q31] 分组后过滤
来源：http://sw.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nv.hahajie.cn

[Q32] 分组拼接字符串
来源：http://st.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mi.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tb.lnxyls.cn

[Q33] 多列分组
来源：http://vu.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bg.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://vu.asd995.cn

SELECT * FROM (
来源：http://dw.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wn.shtwfgs.cn

) t WHERE rn = 1;
来源：http://ry.521024.cn

[Q35] 内连接
来源：http://hz.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://so.hnjuh.cn

[Q36] 左连接
来源：http://yz.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://db.shtwfgs.cn

[Q37] 右连接
来源：http://ki.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ii.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mg.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nq.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://cx.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ez.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ew.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zs.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ew.yuexingan06.cn

[Q41] 多表连接
来源：http://wt.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ca.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://xl.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://in.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://ok.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://xv.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ha.yuexingan06.cn

[Q43] 标量子查询
来源：http://cn.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ar.shxzukj.cn

[Q44] IN 子查询
来源：http://xc.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ej.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://iy.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iq.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tm.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kv.asd995.cn

[Q47] 与平均值比较
来源：http://dh.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ti.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://of.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zu.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://id.hnjuh.cn

[Q49] 更新单行
来源：http://ey.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tz.jianghongdianzi.cn

[Q50] 批量更新
来源：http://ue.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hi.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://re.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zo.nicolike.cn

[Q52] 删除指定行
来源：http://tv.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ed.shxzskj.cn

[Q53] 按条件删除
来源：http://dd.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cn.hahajie.cn

[Q54] 清空表
来源：http://pj.nszjky.cn

TRUNCATE TABLE logs;
来源：http://lh.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://ti.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://so.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ij.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rv.hnjuh.cn

[Q57] 行号
来源：http://xd.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lj.szsharing.cn

[Q58] 累计求和
来源：http://ds.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jm.shxzukj.cn

[Q59] 分组内累计
来源：http://nv.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ug.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://sp.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rr.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pg.nszjky.cn

[Q61] 移动平均
来源：http://st.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ge.gzmigu.cn

[Q62] 分组占比
来源：http://qd.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fz.muxihuayi.cn

[Q63] 开启事务
来源：http://kr.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ef.panjiajie.cn

[Q64] 提交事务
来源：http://ay.nicolike.cn

COMMIT;
来源：http://hs.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://xc.521024.cn

ROLLBACK;
来源：http://ms.haigaiapp.cn

[Q66] 行锁查询
来源：http://du.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://de.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://ii.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pq.shxzskj.cn

[Q68] 保存点
来源：http://zu.muxihuayi.cn

SAVEPOINT sp1;
来源：http://pg.newstarts.cn

ROLLBACK TO sp1;
来源：http://gw.panjiajie.cn

[Q69] 查看执行计划
来源：http://nc.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dd.wgjwhj.cn

[Q70] 更新统计信息
来源：http://gz.shxzukj.cn


<!-- 参考信息 -->