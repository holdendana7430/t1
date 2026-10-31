代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://ik.huixiangedu.cn

Go:   go f()
来源：http://lg.colortex.cn

Ruby: Thread.new { f }
来源：http://nt.huanxung.cn

C#:   Task.Run(() => F());
来源：http://tl.newstarts.cn

[O02] 使用线程池
来源：http://ny.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://el.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://py.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://ad.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://hj.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tx.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ee.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://px.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dw.szsharing.cn

[O03] 加锁保护共享数据
来源：http://cn.lnxyls.cn

Py:   with lock: shared += 1
来源：http://es.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://xs.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ky.bjjhwx.cn

TS:   // 同 JS
来源：http://bp.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://dw.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://io.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oi.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://yk.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://ag.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://bp.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://we.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://oy.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sv.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eo.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zu.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fr.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://hj.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://jq.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://no.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aw.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://ga.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://wp.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qd.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ls.asd995.cn

Ruby: threads.map(&:join)
来源：http://ia.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ch.yuexingan06.cn

[O06] 使用进程池
来源：http://ia.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bk.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tl.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://re.colortex.cn

TS:   // child_process / cluster 模块
来源：http://iv.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ti.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eu.shxzukj.cn

Ruby: // fork 块
来源：http://et.huanxung.cn

C#:   Parallel.For
来源：http://va.huixiangedu.cn

================================================================================
来源：http://tz.bjjhwx.cn

P. 常用工具函数
来源：http://gl.huanxung.cn

================================================================================
来源：http://lp.nszjky.cn

[P01] 生成 UUID
来源：http://ux.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://ed.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yf.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://rz.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://qo.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://gd.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://cz.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://gb.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://tp.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://vz.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jf.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hn.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sv.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hf.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jq.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zi.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ja.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ph.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://ph.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ae.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bv.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zb.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pr.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xi.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uv.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gd.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yv.jctech888.com.cn

[P04] 求长度
来源：http://ln.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://he.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hx.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cs.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qy.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://yr.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://aq.521024.cn

Ruby: x.length;  x.size
来源：http://sg.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lf.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://yn.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tb.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aj.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qo.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oy.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dt.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tu.nszjky.cn

Ruby: a == b
来源：http://sp.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sb.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ta.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cr.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://aj.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pt.panjiajie.cn

TS:   if (x == null) {}
来源：http://qe.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lv.hnjuh.cn

Go:   if x == nil {}
来源：http://gz.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lu.bjjhwx.cn

C#:   if (x is null) {}
来源：http://pl.gzmigu.cn

[P07] 防抖与节流
来源：http://hw.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ei.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://aq.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vf.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jy.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ba.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gw.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rj.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qy.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://yr.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ne.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ys.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zv.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://og.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bc.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fa.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qj.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ci.yuexingan06.cn

================================================================================
来源：http://by.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vo.szxytkj.cn

================================================================================
来源：http://qm.yuntaijiaju.cn

[Q01] 创建表
来源：http://pz.jianghongdianzi.cn

CREATE TABLE users (
来源：http://bs.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://no.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://uv.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://zr.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bm.hahajie.cn

);
来源：http://vt.lnxyls.cn

[Q02] 创建带外键的表
来源：http://ze.lnxyls.cn

CREATE TABLE orders (
来源：http://yg.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nb.nicolike.cn

user_id INT NOT NULL,
来源：http://br.huanxung.cn

amount DECIMAL(10, 2),
来源：http://gz.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://my.gzmigu.cn

);
来源：http://sz.lnxyls.cn

[Q03] 增加列
来源：http://jo.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yy.szxytkj.cn

[Q04] 修改列类型
来源：http://kj.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zd.szsharing.cn

[Q05] 重命名列
来源：http://ik.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ys.chemitech.net.cn

[Q06] 删除列
来源：http://hc.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vx.szxytkj.cn

[Q07] 删除表
来源：http://sr.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://rq.colortex.cn

[Q08] 创建普通索引
来源：http://fs.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ya.newstarts.cn

[Q09] 创建唯一索引
来源：http://jf.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gm.521024.cn

[Q10] 插入单行
来源：http://pk.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ps.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ff.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xp.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://na.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vb.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uu.gzmigu.cn

[Q13] 忽略重复插入
来源：http://yz.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qp.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://ul.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fq.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wr.huixinmuqiang.cn

[Q15] 查询全部
来源：http://bn.lnxyls.cn

SELECT * FROM users;
来源：http://ls.shtwfgs.cn

[Q16] 查询指定列
来源：http://sm.nszjky.cn

SELECT id, name FROM users;
来源：http://sl.gzmigu.cn

[Q17] 条件查询
来源：http://bf.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zv.shtwfgs.cn

[Q18] 模糊匹配
来源：http://xk.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dr.huixinmuqiang.cn

[Q19] 范围查询
来源：http://au.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jl.newstarts.cn

[Q20] IN 列表
来源：http://pl.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yi.jianghongdianzi.cn

[Q21] 空值判断
来源：http://kz.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ak.muxihuayi.cn

[Q22] 排序
来源：http://om.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://al.521024.cn

[Q23] 分页
来源：http://oj.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://go.shxzskj.cn

[Q24] 去重
来源：http://sk.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://ov.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://mn.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ax.asd995.cn

[Q26] 计数
来源：http://qq.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://hw.nicolike.cn

[Q27] 条件计数
来源：http://vi.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nr.yuexingan06.cn

[Q28] 求和与平均
来源：http://nl.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ed.haigaiapp.cn

[Q29] 最大最小值
来源：http://yl.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sy.jctech888.com.cn

[Q30] 分组统计
来源：http://pw.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zs.haigaiapp.cn

[Q31] 分组后过滤
来源：http://je.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rl.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://ic.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://et.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://up.521024.cn

[Q33] 多列分组
来源：http://bj.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yg.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://mf.newstarts.cn

SELECT * FROM (
来源：http://ji.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mx.newstarts.cn

) t WHERE rn = 1;
来源：http://of.shxzskj.cn

[Q35] 内连接
来源：http://ds.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hl.jianghongdianzi.cn

[Q36] 左连接
来源：http://de.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://il.szxytkj.cn

[Q37] 右连接
来源：http://bt.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ze.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ib.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qv.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://qh.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rc.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pl.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nr.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xo.521024.cn

[Q41] 多表连接
来源：http://tz.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uy.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://fl.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ld.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://cq.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://wf.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gm.muxihuayi.cn

[Q43] 标量子查询
来源：http://on.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wm.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://ju.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ys.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://nc.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ka.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://so.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uq.shtwfgs.cn

[Q47] 与平均值比较
来源：http://bu.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cd.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://ft.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dn.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://vd.szxytkj.cn

[Q49] 更新单行
来源：http://zi.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hs.nszjky.cn

[Q50] 批量更新
来源：http://sh.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://im.lnxyls.cn

[Q51] 用子查询更新
来源：http://uf.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ih.9csxet.cn

[Q52] 删除指定行
来源：http://wi.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://lp.wgjwhj.cn

[Q53] 按条件删除
来源：http://fb.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lp.wgjwhj.cn

[Q54] 清空表
来源：http://oc.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://gf.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://fv.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ne.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://tk.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bj.muxihuayi.cn

[Q57] 行号
来源：http://ob.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wm.jctech888.com.cn

[Q58] 累计求和
来源：http://jv.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yo.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://pq.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jr.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ee.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ep.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tc.gzmigu.cn

[Q61] 移动平均
来源：http://op.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wd.hahajie.cn

[Q62] 分组占比
来源：http://gf.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://we.nszjky.cn

[Q63] 开启事务
来源：http://tu.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cy.huixinmuqiang.cn

[Q64] 提交事务
来源：http://cq.9csxet.cn

COMMIT;
来源：http://cg.jctech888.com.cn

[Q65] 回滚事务
来源：http://go.gzmigu.cn

ROLLBACK;
来源：http://jw.szxytkj.cn

[Q66] 行锁查询
来源：http://na.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qc.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://js.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xx.jctech888.com.cn

[Q68] 保存点
来源：http://yc.panjiajie.cn

SAVEPOINT sp1;
来源：http://dn.panjiajie.cn

ROLLBACK TO sp1;
来源：http://uw.lnxyls.cn

[Q69] 查看执行计划
来源：http://oe.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mq.521024.cn

[Q70] 更新统计信息
来源：http://je.chemitech.net.cn

ANALYZE TABLE users;
来源：http://vc.huanxung.cn

[Q71] 查看建表语句
来源：http://lg.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ol.bookmarksfly.cn

[Q72] 查看索引
来源：http://qa.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://ty.shxzukj.cn

[Q73] 查看表状态
来源：http://ar.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mk.hnjuh.cn

[Q74] 强制使用索引
来源：http://hb.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bt.newstarts.cn

[Q75] 日期格式化
来源：http://tk.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ue.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pk.bookmarksfly.cn


<!-- 参考信息 -->