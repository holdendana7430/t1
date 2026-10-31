代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ab.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://id.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yn.nicolike.cn

TS:   // 同 JS
来源：http://zd.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ez.haigaiapp.cn

Go:   go f()
来源：http://fh.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://wt.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://kg.shxzskj.cn

[O02] 使用线程池
来源：http://xy.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yi.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lr.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://vt.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://od.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zz.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gt.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tl.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cb.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://nf.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://hu.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://ee.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gb.shxzukj.cn

TS:   // 同 JS
来源：http://ri.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://hv.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zz.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zx.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://as.huanxung.cn

[O04] 定义异步函数并等待
来源：http://du.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://ml.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ir.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://jd.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sp.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ww.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ky.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zq.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://fz.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://uf.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://bb.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bg.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://ov.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://do.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ff.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pd.9csxet.cn

Ruby: threads.map(&:join)
来源：http://vl.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://os.wgjwhj.cn

[O06] 使用进程池
来源：http://mg.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xt.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ub.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://nq.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://ps.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cn.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zn.shxzukj.cn

Ruby: // fork 块
来源：http://km.szsharing.cn

C#:   Parallel.For
来源：http://hc.shxzskj.cn

================================================================================
来源：http://du.yuntaijiaju.cn

P. 常用工具函数
来源：http://al.huixinmuqiang.cn

================================================================================
来源：http://hk.muxihuayi.cn

[P01] 生成 UUID
来源：http://my.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://iw.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uu.521024.cn

JS:   crypto.randomUUID()
来源：http://ea.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://xn.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://cu.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://lt.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://uw.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://qc.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://nc.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pi.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bo.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://db.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nr.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oo.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mx.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rg.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tr.shxzukj.cn

[P03] 生成短随机字符串
来源：http://ii.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nx.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qf.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ki.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zi.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tb.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gk.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cw.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fw.9csxet.cn

[P04] 求长度
来源：http://kj.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sq.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kg.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uq.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ik.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://op.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://sk.hnjuh.cn

Ruby: x.length;  x.size
来源：http://fb.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pl.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://ff.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ao.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sm.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qz.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ni.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wl.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pl.shtwfgs.cn

Ruby: a == b
来源：http://gt.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bz.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wh.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ab.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://rl.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ud.huixiangedu.cn

TS:   if (x == null) {}
来源：http://qu.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ad.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://yc.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zs.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://ox.9csxet.cn

[P07] 防抖与节流
来源：http://ye.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dg.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ms.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ap.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://og.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hv.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zt.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://md.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gt.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://nt.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hc.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ry.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wb.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rh.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hu.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gd.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nc.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://li.bjjhwx.cn

================================================================================
来源：http://gt.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ch.szxytkj.cn

================================================================================
来源：http://hw.huanxung.cn

[Q01] 创建表
来源：http://ba.muxihuayi.cn

CREATE TABLE users (
来源：http://jk.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zb.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://ta.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://uj.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ys.jctech888.com.cn

);
来源：http://cn.szxytkj.cn

[Q02] 创建带外键的表
来源：http://uo.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://gf.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tv.nicolike.cn

user_id INT NOT NULL,
来源：http://hi.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://as.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ge.hnjuh.cn

);
来源：http://zp.huixinmuqiang.cn

[Q03] 增加列
来源：http://cy.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rf.521024.cn

[Q04] 修改列类型
来源：http://zm.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uu.wgjwhj.cn

[Q05] 重命名列
来源：http://hp.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qn.newstarts.cn

[Q06] 删除列
来源：http://ed.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qw.yuntaijiaju.cn

[Q07] 删除表
来源：http://lw.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://rc.521024.cn

[Q08] 创建普通索引
来源：http://kj.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bb.521024.cn

[Q09] 创建唯一索引
来源：http://de.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bu.nicolike.cn

[Q10] 插入单行
来源：http://qo.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://px.shxzskj.cn

[Q11] 一次插入多行
来源：http://ez.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ft.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://ew.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wg.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bk.panjiajie.cn

[Q13] 忽略重复插入
来源：http://tw.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fy.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://wx.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ej.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kh.gzmigu.cn

[Q15] 查询全部
来源：http://gf.bjjhwx.cn

SELECT * FROM users;
来源：http://di.jctech888.com.cn

[Q16] 查询指定列
来源：http://pf.shtwfgs.cn

SELECT id, name FROM users;
来源：http://yj.lnxyls.cn

[Q17] 条件查询
来源：http://xx.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zo.wgjwhj.cn

[Q18] 模糊匹配
来源：http://xo.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pe.asd995.cn

[Q19] 范围查询
来源：http://bs.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yn.panjiajie.cn

[Q20] IN 列表
来源：http://ux.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wf.9csxet.cn

[Q21] 空值判断
来源：http://ll.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bz.yuexingan06.cn

[Q22] 排序
来源：http://pn.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ts.huixinmuqiang.cn

[Q23] 分页
来源：http://nx.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hd.haigaiapp.cn

[Q24] 去重
来源：http://cw.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://jp.hnjuh.cn

[Q25] 只取前 N 条
来源：http://ut.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yk.huanxung.cn

[Q26] 计数
来源：http://rh.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://lc.huanxung.cn

[Q27] 条件计数
来源：http://it.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nj.asd995.cn

[Q28] 求和与平均
来源：http://lb.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rq.nicolike.cn

[Q29] 最大最小值
来源：http://qx.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qz.szsharing.cn

[Q30] 分组统计
来源：http://wn.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ut.panjiajie.cn

[Q31] 分组后过滤
来源：http://qu.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ey.nicolike.cn

[Q32] 分组拼接字符串
来源：http://ia.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://os.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ny.huanxung.cn

[Q33] 多列分组
来源：http://ng.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nc.521024.cn

[Q34] 每组取第一条
来源：http://zd.shxzukj.cn

SELECT * FROM (
来源：http://wr.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dg.shtwfgs.cn

) t WHERE rn = 1;
来源：http://ve.szxytkj.cn

[Q35] 内连接
来源：http://sm.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fy.nszjky.cn

[Q36] 左连接
来源：http://mi.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fd.yuntaijiaju.cn

[Q37] 右连接
来源：http://wf.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dn.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zz.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yh.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://ks.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xm.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ne.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ah.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://is.hnjuh.cn

[Q41] 多表连接
来源：http://rq.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wq.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://vy.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://xn.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ia.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://os.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xd.521024.cn

[Q43] 标量子查询
来源：http://qg.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dn.shxzskj.cn

[Q44] IN 子查询
来源：http://ec.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rd.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://we.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://im.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sx.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ad.szsharing.cn

[Q47] 与平均值比较
来源：http://zp.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wb.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://xk.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gr.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://au.huixiangedu.cn

[Q49] 更新单行
来源：http://iq.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iq.huixiangedu.cn

[Q50] 批量更新
来源：http://rs.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lm.panjiajie.cn

[Q51] 用子查询更新
来源：http://dw.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ox.lnxyls.cn

[Q52] 删除指定行
来源：http://tu.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://fd.chemitech.net.cn

[Q53] 按条件删除
来源：http://uc.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cc.shxzskj.cn

[Q54] 清空表
来源：http://hy.nicolike.cn

TRUNCATE TABLE logs;
来源：http://cr.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://vo.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tt.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://lx.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qd.chemitech.net.cn

[Q57] 行号
来源：http://bk.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qj.bjjhwx.cn

[Q58] 累计求和
来源：http://rc.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qr.lnxyls.cn

[Q59] 分组内累计
来源：http://sl.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dx.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://yw.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qb.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vz.muxihuayi.cn

[Q61] 移动平均
来源：http://bp.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jy.jianghongdianzi.cn

[Q62] 分组占比
来源：http://ty.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zz.szsharing.cn

[Q63] 开启事务
来源：http://xv.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gi.huanxung.cn

[Q64] 提交事务
来源：http://kt.huixiangedu.cn

COMMIT;
来源：http://ea.shxzskj.cn

[Q65] 回滚事务
来源：http://rn.nszjky.cn

ROLLBACK;
来源：http://dw.bjjhwx.cn

[Q66] 行锁查询
来源：http://pm.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uy.asd995.cn

[Q67] 设置隔离级别
来源：http://gz.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yo.huixinmuqiang.cn

[Q68] 保存点
来源：http://kl.hnjuh.cn

SAVEPOINT sp1;
来源：http://oy.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://hx.jctech888.com.cn

[Q69] 查看执行计划
来源：http://to.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sg.szxytkj.cn

[Q70] 更新统计信息
来源：http://ax.gzmigu.cn

ANALYZE TABLE users;
来源：http://yd.yuexingan06.cn

[Q71] 查看建表语句
来源：http://wx.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://er.panjiajie.cn

[Q72] 查看索引
来源：http://cu.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://sk.jctech888.com.cn

[Q73] 查看表状态
来源：http://pk.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yy.chemitech.net.cn

[Q74] 强制使用索引
来源：http://sh.bjjhwx.cn


<!-- 参考信息 -->