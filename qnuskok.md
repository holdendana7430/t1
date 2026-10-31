代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wz.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://as.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xx.haigaiapp.cn

TS:   // 同 JS
来源：http://nx.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://kl.jianghongdianzi.cn

Go:   go f()
来源：http://hy.newstarts.cn

Ruby: Thread.new { f }
来源：http://gg.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://al.muxihuayi.cn

[O02] 使用线程池
来源：http://sf.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://js.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lx.521024.cn

JS:   // worker_threads 线程池
来源：http://gl.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://ez.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zw.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fa.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gw.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gu.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://cw.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://hh.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://jy.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qs.szsharing.cn

TS:   // 同 JS
来源：http://ap.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://ou.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ff.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uy.521024.cn

C#:   lock (gate) { shared++; }
来源：http://ux.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://ch.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://tp.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sg.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ff.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wr.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vf.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fc.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rv.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://yj.521024.cn

[O05] 并发执行并等待全部完成
来源：http://kn.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://ch.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sa.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://oo.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://cd.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://us.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ug.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://fc.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oh.yuexingan06.cn

[O06] 使用进程池
来源：http://tc.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wt.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cb.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://sq.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://gv.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wy.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ju.nicolike.cn

Ruby: // fork 块
来源：http://ug.asd995.cn

C#:   Parallel.For
来源：http://sl.szsharing.cn

================================================================================
来源：http://im.newstarts.cn

P. 常用工具函数
来源：http://rp.huixiangedu.cn

================================================================================
来源：http://eh.shxzukj.cn

[P01] 生成 UUID
来源：http://ct.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://tl.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bz.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://sq.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://jd.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://fu.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ny.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://dl.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://sd.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://da.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qi.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qf.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dg.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cw.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kl.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eu.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rw.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jd.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://bf.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jm.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mc.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xm.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nv.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zy.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yj.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pk.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zo.bjjhwx.cn

[P04] 求长度
来源：http://rh.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://um.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xn.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vt.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://de.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://lz.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://bh.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tf.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://zs.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ij.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sn.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cf.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://et.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iy.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lr.bookmarksfly.cn

Ruby: a == b
来源：http://xq.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oj.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kv.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://to.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://rj.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lx.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://qz.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bh.shxzskj.cn

Go:   if x == nil {}
来源：http://gx.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rr.yuexingan06.cn

C#:   if (x is null) {}
来源：http://mt.colortex.cn

[P07] 防抖与节流
来源：http://fu.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eu.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://bq.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jp.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://id.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mx.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ya.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tn.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sm.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://pb.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tn.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cc.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sv.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://es.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zg.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xj.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ss.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ub.gzmigu.cn

================================================================================
来源：http://dd.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uj.szsharing.cn

================================================================================
来源：http://wx.hahajie.cn

[Q01] 创建表
来源：http://ez.newstarts.cn

CREATE TABLE users (
来源：http://ke.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uh.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://of.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://jv.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mx.521024.cn

);
来源：http://yx.szxytkj.cn

[Q02] 创建带外键的表
来源：http://bj.panjiajie.cn

CREATE TABLE orders (
来源：http://rx.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qk.bjjhwx.cn

user_id INT NOT NULL,
来源：http://va.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://ps.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nn.panjiajie.cn

);
来源：http://nn.gzmigu.cn

[Q03] 增加列
来源：http://en.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fn.nicolike.cn

[Q04] 修改列类型
来源：http://zi.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aw.huanxung.cn

[Q05] 重命名列
来源：http://rr.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cy.nicolike.cn

[Q06] 删除列
来源：http://hd.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yi.shtwfgs.cn

[Q07] 删除表
来源：http://ce.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://yq.hahajie.cn

[Q08] 创建普通索引
来源：http://lc.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bp.newstarts.cn

[Q09] 创建唯一索引
来源：http://es.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xd.haigaiapp.cn

[Q10] 插入单行
来源：http://rc.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://es.nicolike.cn

[Q11] 一次插入多行
来源：http://as.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uo.colortex.cn

[Q12] 插入后取自增 ID
来源：http://aj.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gv.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qt.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://kz.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tv.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://wn.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vm.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xl.521024.cn

[Q15] 查询全部
来源：http://gx.muxihuayi.cn

SELECT * FROM users;
来源：http://xg.gzmigu.cn

[Q16] 查询指定列
来源：http://ph.huanxung.cn

SELECT id, name FROM users;
来源：http://gd.szxytkj.cn

[Q17] 条件查询
来源：http://iw.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ax.jctech888.com.cn

[Q18] 模糊匹配
来源：http://dy.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aj.bookmarksfly.cn

[Q19] 范围查询
来源：http://ez.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ck.wgjwhj.cn

[Q20] IN 列表
来源：http://en.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fj.hahajie.cn

[Q21] 空值判断
来源：http://un.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pr.muxihuayi.cn

[Q22] 排序
来源：http://hi.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fv.wgjwhj.cn

[Q23] 分页
来源：http://cz.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kd.bjjhwx.cn

[Q24] 去重
来源：http://jb.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://sz.szsharing.cn

[Q25] 只取前 N 条
来源：http://rm.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jb.huixinmuqiang.cn

[Q26] 计数
来源：http://wl.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://pu.521024.cn

[Q27] 条件计数
来源：http://aa.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://od.gzmigu.cn

[Q28] 求和与平均
来源：http://kk.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vu.colortex.cn

[Q29] 最大最小值
来源：http://kk.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rq.chemitech.net.cn

[Q30] 分组统计
来源：http://wd.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pz.colortex.cn

[Q31] 分组后过滤
来源：http://gx.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ro.nszjky.cn

[Q32] 分组拼接字符串
来源：http://hr.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zm.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ga.szxytkj.cn

[Q33] 多列分组
来源：http://az.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hx.521024.cn

[Q34] 每组取第一条
来源：http://tc.shtwfgs.cn

SELECT * FROM (
来源：http://ls.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bb.wgjwhj.cn

) t WHERE rn = 1;
来源：http://ce.jianghongdianzi.cn

[Q35] 内连接
来源：http://og.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://at.hnjuh.cn

[Q36] 左连接
来源：http://tw.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hw.haigaiapp.cn

[Q37] 右连接
来源：http://wg.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://li.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sn.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kb.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://wj.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ho.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tj.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://om.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ao.nicolike.cn

[Q41] 多表连接
来源：http://oh.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hu.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://sf.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://gc.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://al.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://xu.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lp.yuexingan06.cn

[Q43] 标量子查询
来源：http://pk.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cp.hahajie.cn

[Q44] IN 子查询
来源：http://wt.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dn.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://qp.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gy.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wm.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zw.asd995.cn

[Q47] 与平均值比较
来源：http://up.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zb.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://nv.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xx.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://an.haigaiapp.cn

[Q49] 更新单行
来源：http://vu.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mi.huanxung.cn

[Q50] 批量更新
来源：http://ln.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lh.chemitech.net.cn

[Q51] 用子查询更新
来源：http://bj.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yu.hnjuh.cn

[Q52] 删除指定行
来源：http://cv.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://lr.wgjwhj.cn

[Q53] 按条件删除
来源：http://wg.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lu.nicolike.cn

[Q54] 清空表
来源：http://pe.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://fo.huanxung.cn

[Q55] 排名（并列占位）
来源：http://tr.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sa.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://tu.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bo.muxihuayi.cn

[Q57] 行号
来源：http://sh.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jj.nszjky.cn

[Q58] 累计求和
来源：http://ug.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tn.panjiajie.cn

[Q59] 分组内累计
来源：http://wa.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yi.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://ob.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cb.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wl.nszjky.cn

[Q61] 移动平均
来源：http://gq.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oi.yuexingan06.cn

[Q62] 分组占比
来源：http://ai.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dq.nicolike.cn

[Q63] 开启事务
来源：http://eu.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nk.szxytkj.cn

[Q64] 提交事务
来源：http://es.muxihuayi.cn

COMMIT;
来源：http://qt.shxzskj.cn

[Q65] 回滚事务
来源：http://se.nicolike.cn

ROLLBACK;
来源：http://au.haigaiapp.cn

[Q66] 行锁查询
来源：http://al.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pu.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://qf.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nh.muxihuayi.cn

[Q68] 保存点
来源：http://bw.huanxung.cn

SAVEPOINT sp1;
来源：http://dv.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://mh.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://xr.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jh.jctech888.com.cn

[Q70] 更新统计信息
来源：http://em.shxzskj.cn

ANALYZE TABLE users;
来源：http://tw.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://be.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uw.colortex.cn

[Q72] 查看索引
来源：http://to.szsharing.cn

SHOW INDEX FROM users;
来源：http://vu.szsharing.cn

[Q73] 查看表状态
来源：http://qz.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hj.wgjwhj.cn

[Q74] 强制使用索引
来源：http://ip.yuntaijiaju.cn


<!-- 参考信息 -->