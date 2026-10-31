代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://et.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ot.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ju.521024.cn

TS:   // 同 JS
来源：http://gt.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://dh.yuntaijiaju.cn

Go:   go f()
来源：http://oj.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://sc.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://ct.bookmarksfly.cn

[O02] 使用线程池
来源：http://qg.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yx.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fv.asd995.cn

JS:   // worker_threads 线程池
来源：http://ul.newstarts.cn

TS:   // worker_threads 线程池
来源：http://xt.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ve.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ra.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nf.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fb.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://pk.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://yg.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://lk.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bd.hahajie.cn

TS:   // 同 JS
来源：http://ql.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://lv.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ek.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://db.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://yf.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://lc.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://cg.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ki.newstarts.cn

JS:   async function f() { await g(); }
来源：http://zx.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pt.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hv.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://in.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zw.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://im.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://yf.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://lt.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zi.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://to.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://um.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ye.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ns.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://lf.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ko.hnjuh.cn

[O06] 使用进程池
来源：http://tl.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://re.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bx.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://al.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://sa.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pe.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tt.nicolike.cn

Ruby: // fork 块
来源：http://wz.bjjhwx.cn

C#:   Parallel.For
来源：http://hn.asd995.cn

================================================================================
来源：http://qd.asd995.cn

P. 常用工具函数
来源：http://hr.9csxet.cn

================================================================================
来源：http://qh.521024.cn

[P01] 生成 UUID
来源：http://bc.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://lt.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pi.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://vm.newstarts.cn

TS:   crypto.randomUUID()
来源：http://yq.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://ji.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://cs.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ay.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://qm.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://ns.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://va.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wv.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nq.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sv.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://le.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cn.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lp.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ug.shxzukj.cn

[P03] 生成短随机字符串
来源：http://fc.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sz.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jv.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yo.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ke.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://st.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fd.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mi.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ne.panjiajie.cn

[P04] 求长度
来源：http://sl.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rt.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sr.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xt.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zv.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://yb.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://ln.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://vo.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wa.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://dr.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wq.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jy.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vb.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qx.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lx.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ig.wgjwhj.cn

Ruby: a == b
来源：http://ct.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qd.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://at.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qn.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://na.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hj.chemitech.net.cn

TS:   if (x == null) {}
来源：http://gc.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://we.nicolike.cn

Go:   if x == nil {}
来源：http://za.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tv.shxzukj.cn

C#:   if (x is null) {}
来源：http://hr.szxytkj.cn

[P07] 防抖与节流
来源：http://pu.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bb.521024.cn

PHP:  // 手写时间戳比较
来源：http://iu.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dy.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gh.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cj.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xp.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gv.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tb.huanxung.cn

[P08] 处理浮点精度问题
来源：http://xj.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mi.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zg.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dz.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ge.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://td.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sd.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ww.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ko.lnxyls.cn

================================================================================
来源：http://mj.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hk.newstarts.cn

================================================================================
来源：http://ep.lnxyls.cn

[Q01] 创建表
来源：http://bg.muxihuayi.cn

CREATE TABLE users (
来源：http://ua.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iy.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://uk.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://up.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qq.gzmigu.cn

);
来源：http://eo.nszjky.cn

[Q02] 创建带外键的表
来源：http://kb.huanxung.cn

CREATE TABLE orders (
来源：http://yo.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gs.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://ef.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://kd.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xn.bjjhwx.cn

);
来源：http://vg.hahajie.cn

[Q03] 增加列
来源：http://uf.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ry.shtwfgs.cn

[Q04] 修改列类型
来源：http://dq.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aw.bjjhwx.cn

[Q05] 重命名列
来源：http://nd.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jn.huixiangedu.cn

[Q06] 删除列
来源：http://qf.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ft.newstarts.cn

[Q07] 删除表
来源：http://kk.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://og.haigaiapp.cn

[Q08] 创建普通索引
来源：http://mx.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pk.shxzukj.cn

[Q09] 创建唯一索引
来源：http://qv.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lw.nicolike.cn

[Q10] 插入单行
来源：http://qo.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oz.yuexingan06.cn

[Q11] 一次插入多行
来源：http://tt.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sg.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://ec.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rh.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://di.szxytkj.cn

[Q13] 忽略重复插入
来源：http://pj.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lo.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://xf.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eo.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ad.panjiajie.cn

[Q15] 查询全部
来源：http://rl.yuntaijiaju.cn

SELECT * FROM users;
来源：http://bw.lnxyls.cn

[Q16] 查询指定列
来源：http://py.szxytkj.cn

SELECT id, name FROM users;
来源：http://sf.szsharing.cn

[Q17] 条件查询
来源：http://zy.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pa.haigaiapp.cn

[Q18] 模糊匹配
来源：http://mo.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ci.nszjky.cn

[Q19] 范围查询
来源：http://cf.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ud.jianghongdianzi.cn

[Q20] IN 列表
来源：http://fz.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iz.szsharing.cn

[Q21] 空值判断
来源：http://yy.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rc.yuexingan06.cn

[Q22] 排序
来源：http://mn.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://of.szsharing.cn

[Q23] 分页
来源：http://gl.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fx.szsharing.cn

[Q24] 去重
来源：http://uy.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://lv.shxzskj.cn

[Q25] 只取前 N 条
来源：http://ds.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ua.yuntaijiaju.cn

[Q26] 计数
来源：http://dg.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://gp.bjjhwx.cn

[Q27] 条件计数
来源：http://us.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hm.9csxet.cn

[Q28] 求和与平均
来源：http://yc.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bk.shxzukj.cn

[Q29] 最大最小值
来源：http://bd.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ah.nicolike.cn

[Q30] 分组统计
来源：http://cx.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lc.521024.cn

[Q31] 分组后过滤
来源：http://bh.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ps.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://dg.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mi.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rn.hahajie.cn

[Q33] 多列分组
来源：http://le.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://is.muxihuayi.cn

[Q34] 每组取第一条
来源：http://yy.hahajie.cn

SELECT * FROM (
来源：http://gm.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ek.gzmigu.cn

) t WHERE rn = 1;
来源：http://cd.jctech888.com.cn

[Q35] 内连接
来源：http://zr.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wd.shtwfgs.cn

[Q36] 左连接
来源：http://sd.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hb.huanxung.cn

[Q37] 右连接
来源：http://wh.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hq.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ub.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kd.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://jx.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xi.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ld.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://of.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oe.nicolike.cn

[Q41] 多表连接
来源：http://vt.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zw.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://qd.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://ar.colortex.cn

[Q42] 连接条件附加过滤
来源：http://lz.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://yl.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lf.huanxung.cn

[Q43] 标量子查询
来源：http://lt.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sg.nszjky.cn

[Q44] IN 子查询
来源：http://xa.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qg.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://so.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ut.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://th.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bj.szsharing.cn

[Q47] 与平均值比较
来源：http://bs.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://il.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://yz.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pa.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://om.yuexingan06.cn

[Q49] 更新单行
来源：http://jn.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hq.jctech888.com.cn

[Q50] 批量更新
来源：http://uw.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xz.hnjuh.cn

[Q51] 用子查询更新
来源：http://zj.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kb.lnxyls.cn

[Q52] 删除指定行
来源：http://vt.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://ka.haigaiapp.cn

[Q53] 按条件删除
来源：http://zq.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hq.newstarts.cn

[Q54] 清空表
来源：http://rn.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://rl.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://ft.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qa.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://ca.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lz.wgjwhj.cn

[Q57] 行号
来源：http://zf.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eb.shtwfgs.cn

[Q58] 累计求和
来源：http://tt.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wp.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://xy.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bx.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://pq.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nn.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jf.newstarts.cn

[Q61] 移动平均
来源：http://bw.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xf.haigaiapp.cn

[Q62] 分组占比
来源：http://zs.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kg.9csxet.cn

[Q63] 开启事务
来源：http://xm.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vp.wgjwhj.cn

[Q64] 提交事务
来源：http://vu.huixiangedu.cn

COMMIT;
来源：http://jz.bookmarksfly.cn

[Q65] 回滚事务
来源：http://zi.shxzukj.cn

ROLLBACK;
来源：http://sb.jctech888.com.cn

[Q66] 行锁查询
来源：http://gd.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nc.newstarts.cn

[Q67] 设置隔离级别
来源：http://fa.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ol.521024.cn

[Q68] 保存点
来源：http://wy.szsharing.cn

SAVEPOINT sp1;
来源：http://ry.asd995.cn

ROLLBACK TO sp1;
来源：http://ke.szxytkj.cn

[Q69] 查看执行计划
来源：http://gu.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yk.muxihuayi.cn

[Q70] 更新统计信息
来源：http://du.hnjuh.cn

ANALYZE TABLE users;
来源：http://pi.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://xd.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gj.szxytkj.cn

[Q72] 查看索引
来源：http://jl.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://cd.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://sf.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kr.shtwfgs.cn

[Q74] 强制使用索引
来源：http://ds.haigaiapp.cn


<!-- 参考信息 -->