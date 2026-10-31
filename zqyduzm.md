代发 wailian999

================================================================================
来源：http://bk.hnjuh.cn

O. 并发与异步
来源：http://jf.bjjhwx.cn

================================================================================
来源：http://xf.shxzskj.cn

[O01] 启动一个线程
来源：http://fg.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fx.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yo.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vn.hahajie.cn

TS:   // 同 JS
来源：http://pd.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://kw.nszjky.cn

Go:   go f()
来源：http://mc.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://wd.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://ax.nszjky.cn

[O02] 使用线程池
来源：http://me.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pk.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lh.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://um.newstarts.cn

TS:   // worker_threads 线程池
来源：http://uq.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://et.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ts.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://is.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ii.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://af.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://ul.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://va.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pq.asd995.cn

TS:   // 同 JS
来源：http://hi.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://zw.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nh.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wv.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://bi.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://tn.521024.cn

Py:   async def f():⏎    await g()
来源：http://tv.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mb.asd995.cn

JS:   async function f() { await g(); }
来源：http://cs.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fd.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kp.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hw.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bj.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://lx.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://dd.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://jy.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://io.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://ep.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://ss.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uo.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bd.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://uh.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ex.jianghongdianzi.cn

[O06] 使用进程池
来源：http://lt.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bn.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cb.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://lt.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://pf.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sx.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dw.chemitech.net.cn

Ruby: // fork 块
来源：http://jx.huixiangedu.cn

C#:   Parallel.For
来源：http://xp.hnjuh.cn

================================================================================
来源：http://hm.asd995.cn

P. 常用工具函数
来源：http://iq.bjjhwx.cn

================================================================================
来源：http://iv.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://om.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://lq.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fm.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://jo.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://ev.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://sw.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://lb.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ew.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://js.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://hk.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wh.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tw.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ca.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sr.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kk.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://md.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dg.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ql.hahajie.cn

[P03] 生成短随机字符串
来源：http://gx.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ep.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://su.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ii.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kk.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pr.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zi.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wh.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gu.jianghongdianzi.cn

[P04] 求长度
来源：http://um.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ah.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sn.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tk.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://in.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://ns.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://mc.nicolike.cn

Ruby: x.length;  x.size
来源：http://vd.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qk.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://xt.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sp.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://md.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fr.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qd.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ms.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xp.chemitech.net.cn

Ruby: a == b
来源：http://af.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pd.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sj.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dj.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ip.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gm.shxzukj.cn

TS:   if (x == null) {}
来源：http://ur.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fg.521024.cn

Go:   if x == nil {}
来源：http://ox.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wd.asd995.cn

C#:   if (x is null) {}
来源：http://fh.huixiangedu.cn

[P07] 防抖与节流
来源：http://hb.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kx.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://ng.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cf.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aq.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://me.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ng.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bu.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kq.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://sg.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lp.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zb.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rs.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dr.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ku.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ui.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tj.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kl.huixiangedu.cn

================================================================================
来源：http://jx.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jm.nicolike.cn

================================================================================
来源：http://vc.wgjwhj.cn

[Q01] 创建表
来源：http://bx.newstarts.cn

CREATE TABLE users (
来源：http://qa.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tj.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://bi.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://zl.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rv.haigaiapp.cn

);
来源：http://dz.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://yh.hnjuh.cn

CREATE TABLE orders (
来源：http://zg.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ym.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://os.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://zz.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oo.nicolike.cn

);
来源：http://rz.haigaiapp.cn

[Q03] 增加列
来源：http://kq.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fc.yuexingan06.cn

[Q04] 修改列类型
来源：http://td.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xs.newstarts.cn

[Q05] 重命名列
来源：http://fx.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kq.hahajie.cn

[Q06] 删除列
来源：http://ag.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tz.hnjuh.cn

[Q07] 删除表
来源：http://ce.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://ss.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://rn.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nt.colortex.cn

[Q09] 创建唯一索引
来源：http://bk.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sj.shxzukj.cn

[Q10] 插入单行
来源：http://fa.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nv.hahajie.cn

[Q11] 一次插入多行
来源：http://ia.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xp.521024.cn

[Q12] 插入后取自增 ID
来源：http://eb.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vi.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vt.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://lt.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ts.521024.cn

[Q14] 存在则更新（upsert）
来源：http://hr.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://be.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oc.shxzskj.cn

[Q15] 查询全部
来源：http://kk.shtwfgs.cn

SELECT * FROM users;
来源：http://uk.asd995.cn

[Q16] 查询指定列
来源：http://oh.521024.cn

SELECT id, name FROM users;
来源：http://nk.bjjhwx.cn

[Q17] 条件查询
来源：http://gu.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fe.nszjky.cn

[Q18] 模糊匹配
来源：http://jg.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pc.muxihuayi.cn

[Q19] 范围查询
来源：http://iv.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://up.nszjky.cn

[Q20] IN 列表
来源：http://ma.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zs.huanxung.cn

[Q21] 空值判断
来源：http://hy.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wo.huixinmuqiang.cn

[Q22] 排序
来源：http://gd.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jl.jctech888.com.cn

[Q23] 分页
来源：http://pc.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bo.huixinmuqiang.cn

[Q24] 去重
来源：http://lp.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://zp.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://rc.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://om.szxytkj.cn

[Q26] 计数
来源：http://eb.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://zo.hahajie.cn

[Q27] 条件计数
来源：http://ck.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bz.nszjky.cn

[Q28] 求和与平均
来源：http://rx.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wc.szsharing.cn

[Q29] 最大最小值
来源：http://rf.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lv.jianghongdianzi.cn

[Q30] 分组统计
来源：http://gn.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pg.jctech888.com.cn

[Q31] 分组后过滤
来源：http://vp.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://da.szsharing.cn

[Q32] 分组拼接字符串
来源：http://an.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lb.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jk.asd995.cn

[Q33] 多列分组
来源：http://pb.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jp.hahajie.cn

[Q34] 每组取第一条
来源：http://up.nicolike.cn

SELECT * FROM (
来源：http://bq.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wx.haigaiapp.cn

) t WHERE rn = 1;
来源：http://hy.nicolike.cn

[Q35] 内连接
来源：http://vs.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lc.nicolike.cn

[Q36] 左连接
来源：http://dw.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zh.yuntaijiaju.cn

[Q37] 右连接
来源：http://lh.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pj.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uc.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://it.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://xz.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yi.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mm.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lw.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qp.colortex.cn

[Q41] 多表连接
来源：http://hf.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ej.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://js.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://fz.asd995.cn

[Q42] 连接条件附加过滤
来源：http://ch.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://tc.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ou.huanxung.cn

[Q43] 标量子查询
来源：http://yr.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ch.huixiangedu.cn

[Q44] IN 子查询
来源：http://ol.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vh.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://mv.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zw.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tn.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gu.colortex.cn

[Q47] 与平均值比较
来源：http://uo.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://le.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://us.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gw.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://yj.gzmigu.cn

[Q49] 更新单行
来源：http://fy.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ya.gzmigu.cn

[Q50] 批量更新
来源：http://nr.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gr.nszjky.cn

[Q51] 用子查询更新
来源：http://qk.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cb.wgjwhj.cn

[Q52] 删除指定行
来源：http://bn.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ni.bjjhwx.cn

[Q53] 按条件删除
来源：http://fn.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://up.jctech888.com.cn

[Q54] 清空表
来源：http://id.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://fg.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://fe.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rh.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://am.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://se.521024.cn

[Q57] 行号
来源：http://bu.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lx.asd995.cn

[Q58] 累计求和
来源：http://dg.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mv.9csxet.cn

[Q59] 分组内累计
来源：http://iw.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ph.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://pw.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ni.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mw.jctech888.com.cn

[Q61] 移动平均
来源：http://hu.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kl.wgjwhj.cn

[Q62] 分组占比
来源：http://bi.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nj.jctech888.com.cn

[Q63] 开启事务
来源：http://hv.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rh.huixinmuqiang.cn

[Q64] 提交事务
来源：http://qi.colortex.cn

COMMIT;
来源：http://yw.bookmarksfly.cn

[Q65] 回滚事务
来源：http://dl.shtwfgs.cn

ROLLBACK;
来源：http://dz.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://qx.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hk.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://nq.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wi.521024.cn

[Q68] 保存点
来源：http://sf.colortex.cn

SAVEPOINT sp1;
来源：http://ng.huanxung.cn

ROLLBACK TO sp1;
来源：http://dw.gzmigu.cn

[Q69] 查看执行计划
来源：http://yj.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qc.colortex.cn

[Q70] 更新统计信息
来源：http://jb.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://ax.newstarts.cn

[Q71] 查看建表语句
来源：http://uy.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qd.521024.cn

[Q72] 查看索引
来源：http://cf.chemitech.net.cn


<!-- 参考信息 -->