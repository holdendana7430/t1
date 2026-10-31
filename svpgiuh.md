代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rn.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bv.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tk.hnjuh.cn

TS:   // 同 JS
来源：http://rj.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://un.yuntaijiaju.cn

Go:   go f()
来源：http://rj.hahajie.cn

Ruby: Thread.new { f }
来源：http://rc.szsharing.cn

C#:   Task.Run(() => F());
来源：http://qj.521024.cn

[O02] 使用线程池
来源：http://ia.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ly.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yn.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://cc.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://jj.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qj.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vo.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dj.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uq.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://jh.colortex.cn

Py:   with lock: shared += 1
来源：http://bu.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://bj.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://de.haigaiapp.cn

TS:   // 同 JS
来源：http://bs.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://pq.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jz.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jq.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ti.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://tn.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ih.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://au.9csxet.cn

JS:   async function f() { await g(); }
来源：http://mc.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pq.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wi.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sw.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ty.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://tr.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://gz.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://qt.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kr.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://nd.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://uu.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xo.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mc.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://zo.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rd.huixinmuqiang.cn

[O06] 使用进程池
来源：http://ut.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tn.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://no.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://rj.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://du.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uu.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hx.wgjwhj.cn

Ruby: // fork 块
来源：http://zy.huanxung.cn

C#:   Parallel.For
来源：http://kn.shtwfgs.cn

================================================================================
来源：http://ca.bookmarksfly.cn

P. 常用工具函数
来源：http://fe.gzmigu.cn

================================================================================
来源：http://sj.bookmarksfly.cn

[P01] 生成 UUID
来源：http://kp.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://jk.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bx.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://bf.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://ub.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://ku.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://wn.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://da.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://al.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://ne.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qb.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zy.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wf.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ur.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://az.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yh.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wg.newstarts.cn

[P03] 生成短随机字符串
来源：http://zb.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bq.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lx.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eb.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vr.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pg.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pf.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dg.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ob.shxzukj.cn

[P04] 求长度
来源：http://df.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jc.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cx.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gl.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lj.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://mg.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://hu.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://or.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fo.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://wd.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://to.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ws.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sj.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qk.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pr.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pm.hnjuh.cn

Ruby: a == b
来源：http://or.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uz.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ad.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gu.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://kj.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mi.huanxung.cn

TS:   if (x == null) {}
来源：http://of.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uy.huanxung.cn

Go:   if x == nil {}
来源：http://to.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oy.shxzskj.cn

C#:   if (x is null) {}
来源：http://qy.szsharing.cn

[P07] 防抖与节流
来源：http://ur.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hy.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://fj.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xa.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ca.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sj.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cp.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ox.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nx.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://rq.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dz.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ri.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ym.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aw.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qc.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gc.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jw.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kb.lnxyls.cn

================================================================================
来源：http://hg.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dd.haigaiapp.cn

================================================================================
来源：http://iu.shtwfgs.cn

[Q01] 创建表
来源：http://mj.colortex.cn

CREATE TABLE users (
来源：http://ff.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fp.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://vg.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://vc.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ps.521024.cn

);
来源：http://up.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://zi.wgjwhj.cn

CREATE TABLE orders (
来源：http://rx.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tk.nicolike.cn

user_id INT NOT NULL,
来源：http://ne.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://mf.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sj.shtwfgs.cn

);
来源：http://vw.jianghongdianzi.cn

[Q03] 增加列
来源：http://xs.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lt.haigaiapp.cn

[Q04] 修改列类型
来源：http://iz.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ff.chemitech.net.cn

[Q05] 重命名列
来源：http://ee.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wr.gzmigu.cn

[Q06] 删除列
来源：http://tp.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qw.gzmigu.cn

[Q07] 删除表
来源：http://qt.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://kl.521024.cn

[Q08] 创建普通索引
来源：http://qm.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ud.colortex.cn

[Q09] 创建唯一索引
来源：http://lf.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ur.huanxung.cn

[Q10] 插入单行
来源：http://fq.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jf.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://si.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://re.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://zi.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://un.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ri.shxzskj.cn

[Q13] 忽略重复插入
来源：http://fy.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vq.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://zh.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ux.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yn.521024.cn

[Q15] 查询全部
来源：http://gq.9csxet.cn

SELECT * FROM users;
来源：http://bn.hahajie.cn

[Q16] 查询指定列
来源：http://ot.gzmigu.cn

SELECT id, name FROM users;
来源：http://wd.huanxung.cn

[Q17] 条件查询
来源：http://wf.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wm.szxytkj.cn

[Q18] 模糊匹配
来源：http://ch.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uz.asd995.cn

[Q19] 范围查询
来源：http://gu.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qu.bjjhwx.cn

[Q20] IN 列表
来源：http://xr.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uk.huixiangedu.cn

[Q21] 空值判断
来源：http://kd.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://le.colortex.cn

[Q22] 排序
来源：http://hi.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cc.shxzskj.cn

[Q23] 分页
来源：http://ow.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dm.huixinmuqiang.cn

[Q24] 去重
来源：http://zq.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://bd.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://hh.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oj.jianghongdianzi.cn

[Q26] 计数
来源：http://bp.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://uq.hahajie.cn

[Q27] 条件计数
来源：http://pc.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ww.huixiangedu.cn

[Q28] 求和与平均
来源：http://iu.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bm.shxzukj.cn

[Q29] 最大最小值
来源：http://gj.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gh.chemitech.net.cn

[Q30] 分组统计
来源：http://as.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eq.shxzskj.cn

[Q31] 分组后过滤
来源：http://hj.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ay.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://fp.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xh.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kf.wgjwhj.cn

[Q33] 多列分组
来源：http://zh.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fv.muxihuayi.cn

[Q34] 每组取第一条
来源：http://az.muxihuayi.cn

SELECT * FROM (
来源：http://wv.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rn.colortex.cn

) t WHERE rn = 1;
来源：http://kg.jianghongdianzi.cn

[Q35] 内连接
来源：http://un.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rn.yuexingan06.cn

[Q36] 左连接
来源：http://qi.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bx.shxzukj.cn

[Q37] 右连接
来源：http://ln.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dj.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ym.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://et.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://zi.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://px.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rh.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gb.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hm.bjjhwx.cn

[Q41] 多表连接
来源：http://xo.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yr.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://lp.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://zz.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://lt.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://xo.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wg.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://kh.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ia.haigaiapp.cn

[Q44] IN 子查询
来源：http://zv.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vy.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://go.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ae.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ro.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xt.huanxung.cn

[Q47] 与平均值比较
来源：http://pc.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yq.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://ck.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://em.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://co.hahajie.cn

[Q49] 更新单行
来源：http://nm.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bp.colortex.cn

[Q50] 批量更新
来源：http://vb.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://py.szsharing.cn

[Q51] 用子查询更新
来源：http://to.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gv.nicolike.cn

[Q52] 删除指定行
来源：http://kr.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://th.szsharing.cn

[Q53] 按条件删除
来源：http://lp.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://le.szxytkj.cn

[Q54] 清空表
来源：http://eu.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://kc.huanxung.cn

[Q55] 排名（并列占位）
来源：http://nn.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gh.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://dp.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ed.yuntaijiaju.cn

[Q57] 行号
来源：http://ta.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xq.shtwfgs.cn

[Q58] 累计求和
来源：http://yf.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ek.panjiajie.cn

[Q59] 分组内累计
来源：http://ks.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vz.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://kd.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vj.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zz.huixiangedu.cn

[Q61] 移动平均
来源：http://rn.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fd.hahajie.cn

[Q62] 分组占比
来源：http://rl.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sb.shxzukj.cn

[Q63] 开启事务
来源：http://tm.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eq.chemitech.net.cn

[Q64] 提交事务
来源：http://ij.colortex.cn

COMMIT;
来源：http://gf.huanxung.cn

[Q65] 回滚事务
来源：http://lv.hahajie.cn

ROLLBACK;
来源：http://hh.lnxyls.cn

[Q66] 行锁查询
来源：http://bj.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ih.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://rx.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yd.gzmigu.cn

[Q68] 保存点
来源：http://kk.521024.cn

SAVEPOINT sp1;
来源：http://rd.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://mg.wgjwhj.cn

[Q69] 查看执行计划
来源：http://wl.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ys.newstarts.cn

[Q70] 更新统计信息
来源：http://cd.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://tm.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://ah.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wo.hnjuh.cn

[Q72] 查看索引
来源：http://bj.shxzukj.cn

SHOW INDEX FROM users;
来源：http://po.lnxyls.cn

[Q73] 查看表状态
来源：http://nn.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rv.huanxung.cn

[Q74] 强制使用索引
来源：http://ol.bookmarksfly.cn


<!-- 参考信息 -->