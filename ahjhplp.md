代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://yn.asd995.cn

Go:   go f()
来源：http://ux.colortex.cn

Ruby: Thread.new { f }
来源：http://nn.nicolike.cn

C#:   Task.Run(() => F());
来源：http://oo.chemitech.net.cn

[O02] 使用线程池
来源：http://re.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pl.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lc.huanxung.cn

JS:   // worker_threads 线程池
来源：http://oq.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://fh.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wb.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bl.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qj.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bo.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://qo.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ke.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://qr.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bp.521024.cn

TS:   // 同 JS
来源：http://uj.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://sb.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bq.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mr.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://mx.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://fd.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://wq.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rg.hahajie.cn

JS:   async function f() { await g(); }
来源：http://qm.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xf.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jv.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nb.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ww.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://uy.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://ag.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://ti.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kl.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://ms.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ew.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jp.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vt.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://eg.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://km.hahajie.cn

[O06] 使用进程池
来源：http://iq.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zx.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nm.asd995.cn

JS:   // child_process / cluster 模块
来源：http://yi.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://jf.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ra.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qm.haigaiapp.cn

Ruby: // fork 块
来源：http://cw.huixinmuqiang.cn

C#:   Parallel.For
来源：http://lc.muxihuayi.cn

================================================================================
来源：http://zz.colortex.cn

P. 常用工具函数
来源：http://gh.huanxung.cn

================================================================================
来源：http://aa.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://jm.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://pb.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xw.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://ta.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://zt.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://eq.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://cv.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://un.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ya.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://pg.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uc.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eo.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ou.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eq.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xd.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ja.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qe.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xx.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://zj.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ai.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cz.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://su.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://at.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bl.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hw.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ky.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yl.szsharing.cn

[P04] 求长度
来源：http://rt.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nz.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bm.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cs.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uo.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://uy.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://wi.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://oe.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yt.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://gk.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dx.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dr.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ct.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kz.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sx.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qb.panjiajie.cn

Ruby: a == b
来源：http://sw.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vc.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xe.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jo.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://vg.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gc.shxzskj.cn

TS:   if (x == null) {}
来源：http://xq.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hk.newstarts.cn

Go:   if x == nil {}
来源：http://to.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xs.panjiajie.cn

C#:   if (x is null) {}
来源：http://fp.yuexingan06.cn

[P07] 防抖与节流
来源：http://rl.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zn.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://pd.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://af.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wt.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ux.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nt.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zx.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jm.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://ft.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zj.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ym.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sc.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dg.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://af.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://og.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://be.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ip.jctech888.com.cn

================================================================================
来源：http://dn.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qt.huixiangedu.cn

================================================================================
来源：http://rh.9csxet.cn

[Q01] 创建表
来源：http://xc.521024.cn

CREATE TABLE users (
来源：http://hc.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bx.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://sr.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://ys.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jp.colortex.cn

);
来源：http://gh.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://th.szxytkj.cn

CREATE TABLE orders (
来源：http://st.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cy.chemitech.net.cn

user_id INT NOT NULL,
来源：http://ou.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://ht.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xs.chemitech.net.cn

);
来源：http://bc.szxytkj.cn

[Q03] 增加列
来源：http://rc.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fc.521024.cn

[Q04] 修改列类型
来源：http://bf.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fs.chemitech.net.cn

[Q05] 重命名列
来源：http://ag.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dv.asd995.cn

[Q06] 删除列
来源：http://vn.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cv.szxytkj.cn

[Q07] 删除表
来源：http://aj.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://kp.yuexingan06.cn

[Q08] 创建普通索引
来源：http://db.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ll.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://dm.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uo.chemitech.net.cn

[Q10] 插入单行
来源：http://hs.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vs.shxzukj.cn

[Q11] 一次插入多行
来源：http://hn.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sj.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://qw.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uf.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lc.hahajie.cn

[Q13] 忽略重复插入
来源：http://cr.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pp.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://qu.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zt.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bg.jianghongdianzi.cn

[Q15] 查询全部
来源：http://bi.shxzukj.cn

SELECT * FROM users;
来源：http://pv.bjjhwx.cn

[Q16] 查询指定列
来源：http://cl.shxzukj.cn

SELECT id, name FROM users;
来源：http://vg.jianghongdianzi.cn

[Q17] 条件查询
来源：http://em.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eg.huixiangedu.cn

[Q18] 模糊匹配
来源：http://in.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uz.jctech888.com.cn

[Q19] 范围查询
来源：http://bj.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ow.gzmigu.cn

[Q20] IN 列表
来源：http://bx.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lx.521024.cn

[Q21] 空值判断
来源：http://mq.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dk.jctech888.com.cn

[Q22] 排序
来源：http://eu.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kq.huanxung.cn

[Q23] 分页
来源：http://sr.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jh.lnxyls.cn

[Q24] 去重
来源：http://qs.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://qf.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://fe.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hr.wgjwhj.cn

[Q26] 计数
来源：http://wt.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://qc.yuexingan06.cn

[Q27] 条件计数
来源：http://za.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ll.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://yh.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hf.9csxet.cn

[Q29] 最大最小值
来源：http://gc.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qa.wgjwhj.cn

[Q30] 分组统计
来源：http://zv.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bu.gzmigu.cn

[Q31] 分组后过滤
来源：http://zs.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nm.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://bz.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ak.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uy.asd995.cn

[Q33] 多列分组
来源：http://fe.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zi.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://fz.hahajie.cn

SELECT * FROM (
来源：http://us.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cu.521024.cn

) t WHERE rn = 1;
来源：http://ea.szxytkj.cn

[Q35] 内连接
来源：http://db.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pp.jctech888.com.cn

[Q36] 左连接
来源：http://te.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ei.yuntaijiaju.cn

[Q37] 右连接
来源：http://xe.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ql.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://da.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vw.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://ch.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mm.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pn.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xp.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gq.huixinmuqiang.cn

[Q41] 多表连接
来源：http://vu.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vi.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://am.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://mf.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://xm.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://yk.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://op.521024.cn

[Q43] 标量子查询
来源：http://ej.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ra.9csxet.cn

[Q44] IN 子查询
来源：http://vx.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://em.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://ty.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pz.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bh.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iu.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://fo.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ww.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://ic.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rx.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://rt.bjjhwx.cn

[Q49] 更新单行
来源：http://yt.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vk.haigaiapp.cn

[Q50] 批量更新
来源：http://vw.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dg.muxihuayi.cn

[Q51] 用子查询更新
来源：http://jy.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://su.szsharing.cn

[Q52] 删除指定行
来源：http://vv.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://mn.lnxyls.cn

[Q53] 按条件删除
来源：http://mq.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wz.nszjky.cn

[Q54] 清空表
来源：http://nb.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://pg.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://cj.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mt.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://gr.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://je.hahajie.cn

[Q57] 行号
来源：http://xu.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://im.yuntaijiaju.cn

[Q58] 累计求和
来源：http://yw.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fz.shxzskj.cn

[Q59] 分组内累计
来源：http://en.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pf.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://kd.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qk.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ql.shtwfgs.cn

[Q61] 移动平均
来源：http://av.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jw.9csxet.cn

[Q62] 分组占比
来源：http://ac.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mh.chemitech.net.cn

[Q63] 开启事务
来源：http://nb.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tz.521024.cn

[Q64] 提交事务
来源：http://ex.szxytkj.cn

COMMIT;
来源：http://xv.hnjuh.cn

[Q65] 回滚事务
来源：http://jy.huixiangedu.cn

ROLLBACK;
来源：http://ok.shxzskj.cn

[Q66] 行锁查询
来源：http://xv.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lg.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://sk.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wj.muxihuayi.cn

[Q68] 保存点
来源：http://nq.haigaiapp.cn

SAVEPOINT sp1;
来源：http://oa.shxzskj.cn

ROLLBACK TO sp1;
来源：http://kv.asd995.cn

[Q69] 查看执行计划
来源：http://hg.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ko.szxytkj.cn

[Q70] 更新统计信息
来源：http://ea.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://eq.bjjhwx.cn

[Q71] 查看建表语句
来源：http://ea.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hp.jianghongdianzi.cn

[Q72] 查看索引
来源：http://ux.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://uu.shxzskj.cn

[Q73] 查看表状态
来源：http://wj.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lz.yuexingan06.cn

[Q74] 强制使用索引
来源：http://qp.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vj.bookmarksfly.cn

[Q75] 日期格式化
来源：http://jc.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ta.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nj.shtwfgs.cn


<!-- 参考信息 -->