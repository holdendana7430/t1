代发 wailian999

================================================================================
来源：http://wf.huanxung.cn

O. 并发与异步
来源：http://vf.huixinmuqiang.cn

================================================================================
来源：http://hq.newstarts.cn

[O01] 启动一个线程
来源：http://mx.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tp.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ug.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ys.bookmarksfly.cn

TS:   // 同 JS
来源：http://xo.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://am.huixinmuqiang.cn

Go:   go f()
来源：http://un.9csxet.cn

Ruby: Thread.new { f }
来源：http://rt.hahajie.cn

C#:   Task.Run(() => F());
来源：http://dp.huanxung.cn

[O02] 使用线程池
来源：http://vf.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sm.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kg.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://we.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://yy.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lt.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vh.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hg.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sq.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ub.9csxet.cn

Py:   with lock: shared += 1
来源：http://fn.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://rd.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lx.huixinmuqiang.cn

TS:   // 同 JS
来源：http://mp.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://zq.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bl.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sg.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://dm.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://op.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://af.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dz.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://wf.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zu.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xa.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pa.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://im.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://ug.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://vd.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://lb.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fp.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://xx.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://zt.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zo.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wf.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://fa.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ve.yuexingan06.cn

[O06] 使用进程池
来源：http://fo.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jz.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://im.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://fs.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://pv.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ze.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hq.nicolike.cn

Ruby: // fork 块
来源：http://km.szsharing.cn

C#:   Parallel.For
来源：http://rj.shxzskj.cn

================================================================================
来源：http://fi.szsharing.cn

P. 常用工具函数
来源：http://ms.muxihuayi.cn

================================================================================
来源：http://hu.huixiangedu.cn

[P01] 生成 UUID
来源：http://ua.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://iy.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bo.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://zk.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://sm.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://mj.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://kt.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://wu.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://yx.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://pg.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ew.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ot.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wd.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ug.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aa.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zt.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nv.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uu.lnxyls.cn

[P03] 生成短随机字符串
来源：http://vq.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qq.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vo.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tg.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cx.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ks.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ck.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://he.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rg.huixinmuqiang.cn

[P04] 求长度
来源：http://bj.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fa.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cz.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ko.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zd.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://zw.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://dh.nszjky.cn

Ruby: x.length;  x.size
来源：http://hv.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nj.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://dt.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ev.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hh.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wn.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://by.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ae.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sn.nszjky.cn

Ruby: a == b
来源：http://me.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pp.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bx.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://st.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://vl.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yy.shxzskj.cn

TS:   if (x == null) {}
来源：http://yx.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mf.shtwfgs.cn

Go:   if x == nil {}
来源：http://hv.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ep.huanxung.cn

C#:   if (x is null) {}
来源：http://uy.colortex.cn

[P07] 防抖与节流
来源：http://pp.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vj.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://ne.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mh.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ih.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://to.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mo.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://da.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kw.huanxung.cn

[P08] 处理浮点精度问题
来源：http://qt.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bn.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zi.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mu.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vy.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cg.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://so.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iw.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://im.szsharing.cn

================================================================================
来源：http://ox.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zz.9csxet.cn

================================================================================
来源：http://kr.jianghongdianzi.cn

[Q01] 创建表
来源：http://lj.szsharing.cn

CREATE TABLE users (
来源：http://vr.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bf.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://yw.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://mn.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mg.panjiajie.cn

);
来源：http://pd.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://mq.hnjuh.cn

CREATE TABLE orders (
来源：http://uh.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lr.nicolike.cn

user_id INT NOT NULL,
来源：http://xk.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://te.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qb.shxzukj.cn

);
来源：http://eo.shtwfgs.cn

[Q03] 增加列
来源：http://sv.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bs.muxihuayi.cn

[Q04] 修改列类型
来源：http://yy.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yz.huixiangedu.cn

[Q05] 重命名列
来源：http://qx.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://na.yuexingan06.cn

[Q06] 删除列
来源：http://ye.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fi.muxihuayi.cn

[Q07] 删除表
来源：http://zo.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://up.huanxung.cn

[Q08] 创建普通索引
来源：http://ef.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://km.shxzukj.cn

[Q09] 创建唯一索引
来源：http://ec.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wr.bjjhwx.cn

[Q10] 插入单行
来源：http://oz.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://es.colortex.cn

[Q11] 一次插入多行
来源：http://ki.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://me.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://km.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xv.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pa.nicolike.cn

[Q13] 忽略重复插入
来源：http://vb.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ol.521024.cn

[Q14] 存在则更新（upsert）
来源：http://ud.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vq.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lz.yuntaijiaju.cn

[Q15] 查询全部
来源：http://wq.jianghongdianzi.cn

SELECT * FROM users;
来源：http://ac.panjiajie.cn

[Q16] 查询指定列
来源：http://fd.jctech888.com.cn

SELECT id, name FROM users;
来源：http://om.nszjky.cn

[Q17] 条件查询
来源：http://jf.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://re.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://dh.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jn.9csxet.cn

[Q19] 范围查询
来源：http://rl.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jf.chemitech.net.cn

[Q20] IN 列表
来源：http://sj.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xf.nszjky.cn

[Q21] 空值判断
来源：http://gt.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lx.huixinmuqiang.cn

[Q22] 排序
来源：http://bo.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vi.gzmigu.cn

[Q23] 分页
来源：http://nn.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kf.9csxet.cn

[Q24] 去重
来源：http://if.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://oo.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://pk.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mf.lnxyls.cn

[Q26] 计数
来源：http://tx.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://se.huixiangedu.cn

[Q27] 条件计数
来源：http://ph.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mn.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://yq.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hf.asd995.cn

[Q29] 最大最小值
来源：http://il.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mg.bookmarksfly.cn

[Q30] 分组统计
来源：http://yh.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vn.huanxung.cn

[Q31] 分组后过滤
来源：http://bf.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ho.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://ln.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zt.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dt.colortex.cn

[Q33] 多列分组
来源：http://gy.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pd.gzmigu.cn

[Q34] 每组取第一条
来源：http://qm.shxzukj.cn

SELECT * FROM (
来源：http://lq.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zl.gzmigu.cn

) t WHERE rn = 1;
来源：http://zk.nicolike.cn

[Q35] 内连接
来源：http://ff.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rg.lnxyls.cn

[Q36] 左连接
来源：http://ld.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wl.shxzskj.cn

[Q37] 右连接
来源：http://gi.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uu.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nz.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ov.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://kw.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hm.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wm.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jo.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gr.muxihuayi.cn

[Q41] 多表连接
来源：http://yq.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ur.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://jt.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://gd.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://xf.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://km.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iy.521024.cn

[Q43] 标量子查询
来源：http://ys.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gf.bjjhwx.cn

[Q44] IN 子查询
来源：http://uu.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rf.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://et.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fl.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fs.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nz.wgjwhj.cn

[Q47] 与平均值比较
来源：http://lv.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hu.521024.cn

[Q48] CTE 公用表表达式
来源：http://gr.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ep.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://yg.huixinmuqiang.cn

[Q49] 更新单行
来源：http://uh.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mj.asd995.cn

[Q50] 批量更新
来源：http://ba.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lb.nszjky.cn

[Q51] 用子查询更新
来源：http://bh.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mn.colortex.cn

[Q52] 删除指定行
来源：http://vz.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://wu.bjjhwx.cn

[Q53] 按条件删除
来源：http://dv.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://az.9csxet.cn

[Q54] 清空表
来源：http://gq.nicolike.cn

TRUNCATE TABLE logs;
来源：http://av.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://pl.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xe.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://xv.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://of.huixiangedu.cn

[Q57] 行号
来源：http://vp.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lh.panjiajie.cn

[Q58] 累计求和
来源：http://ju.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lf.gzmigu.cn

[Q59] 分组内累计
来源：http://iq.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vo.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://su.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ez.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uf.shtwfgs.cn

[Q61] 移动平均
来源：http://ew.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fv.yuntaijiaju.cn

[Q62] 分组占比
来源：http://ys.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ub.asd995.cn

[Q63] 开启事务
来源：http://hz.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fd.bookmarksfly.cn

[Q64] 提交事务
来源：http://wv.lnxyls.cn

COMMIT;
来源：http://mt.jctech888.com.cn

[Q65] 回滚事务
来源：http://nc.9csxet.cn

ROLLBACK;
来源：http://dm.nicolike.cn

[Q66] 行锁查询
来源：http://su.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pc.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://ko.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ya.bookmarksfly.cn

[Q68] 保存点
来源：http://wz.shxzukj.cn

SAVEPOINT sp1;
来源：http://us.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://fc.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://xj.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sd.shxzskj.cn

[Q70] 更新统计信息
来源：http://hq.wgjwhj.cn

ANALYZE TABLE users;
来源：http://gb.gzmigu.cn

[Q71] 查看建表语句
来源：http://nu.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fr.gzmigu.cn

[Q72] 查看索引
来源：http://sk.huixiangedu.cn


<!-- 参考信息 -->