代发 wailian999

TS:   // worker_threads 线程池
来源：http://pl.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qs.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dv.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zt.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ns.hahajie.cn

[O03] 加锁保护共享数据
来源：http://wf.hnjuh.cn

Py:   with lock: shared += 1
来源：http://ml.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://ja.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bz.szsharing.cn

TS:   // 同 JS
来源：http://vq.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://am.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rk.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fm.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://cd.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://pc.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://vv.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qj.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://nz.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xv.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ic.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iz.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ir.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://eg.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://xm.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://wi.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kp.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://rw.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://vc.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://om.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xm.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://mc.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wq.szsharing.cn

[O06] 使用进程池
来源：http://ar.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://on.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xf.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://pn.colortex.cn

TS:   // child_process / cluster 模块
来源：http://ta.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wl.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ci.lnxyls.cn

Ruby: // fork 块
来源：http://ye.chemitech.net.cn

C#:   Parallel.For
来源：http://lr.yuexingan06.cn

================================================================================
来源：http://ic.hahajie.cn

P. 常用工具函数
来源：http://zw.haigaiapp.cn

================================================================================
来源：http://jy.jctech888.com.cn

[P01] 生成 UUID
来源：http://tz.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://pr.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bb.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://ds.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://jd.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://vf.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://xg.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://zd.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://vc.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://kh.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lr.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jw.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xc.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jw.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zu.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://be.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oo.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ev.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://gk.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kf.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://me.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dc.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wo.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gr.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ga.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jj.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iu.huanxung.cn

[P04] 求长度
来源：http://em.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ao.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ki.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xi.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fj.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://iq.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://me.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://kl.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yk.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://yc.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lc.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kh.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lr.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sr.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mi.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nl.szsharing.cn

Ruby: a == b
来源：http://dx.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://my.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sg.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nd.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://ov.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vx.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://se.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ez.bookmarksfly.cn

Go:   if x == nil {}
来源：http://mh.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vz.lnxyls.cn

C#:   if (x is null) {}
来源：http://gh.shtwfgs.cn

[P07] 防抖与节流
来源：http://lg.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nd.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://wt.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ki.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fd.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vi.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yz.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mv.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iz.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://hp.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zx.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vx.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hh.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bp.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cd.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hb.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zv.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://un.bookmarksfly.cn

================================================================================
来源：http://gc.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ew.521024.cn

================================================================================
来源：http://uc.huanxung.cn

[Q01] 创建表
来源：http://ep.jianghongdianzi.cn

CREATE TABLE users (
来源：http://hv.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://me.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ks.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ax.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yy.colortex.cn

);
来源：http://if.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://rs.panjiajie.cn

CREATE TABLE orders (
来源：http://iy.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kk.9csxet.cn

user_id INT NOT NULL,
来源：http://qp.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://cn.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rc.szxytkj.cn

);
来源：http://pn.szsharing.cn

[Q03] 增加列
来源：http://vx.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ai.szxytkj.cn

[Q04] 修改列类型
来源：http://ly.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ab.yuexingan06.cn

[Q05] 重命名列
来源：http://xy.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://by.szxytkj.cn

[Q06] 删除列
来源：http://is.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fj.yuntaijiaju.cn

[Q07] 删除表
来源：http://sj.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://dv.shtwfgs.cn

[Q08] 创建普通索引
来源：http://qp.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nm.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://uf.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ay.gzmigu.cn

[Q10] 插入单行
来源：http://fn.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mf.shtwfgs.cn

[Q11] 一次插入多行
来源：http://pd.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rf.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://fr.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ov.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tx.gzmigu.cn

[Q13] 忽略重复插入
来源：http://dj.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wc.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://tq.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hp.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ax.szsharing.cn

[Q15] 查询全部
来源：http://ij.huixinmuqiang.cn

SELECT * FROM users;
来源：http://of.asd995.cn

[Q16] 查询指定列
来源：http://pg.nszjky.cn

SELECT id, name FROM users;
来源：http://uh.nicolike.cn

[Q17] 条件查询
来源：http://ql.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hl.lnxyls.cn

[Q18] 模糊匹配
来源：http://jm.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rg.panjiajie.cn

[Q19] 范围查询
来源：http://an.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rv.chemitech.net.cn

[Q20] IN 列表
来源：http://vv.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pg.shxzskj.cn

[Q21] 空值判断
来源：http://wu.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sn.jctech888.com.cn

[Q22] 排序
来源：http://mb.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xf.chemitech.net.cn

[Q23] 分页
来源：http://nz.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://or.huixiangedu.cn

[Q24] 去重
来源：http://zo.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://vp.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://ht.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zt.asd995.cn

[Q26] 计数
来源：http://dm.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://hb.nszjky.cn

[Q27] 条件计数
来源：http://xv.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fy.colortex.cn

[Q28] 求和与平均
来源：http://uj.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uw.hnjuh.cn

[Q29] 最大最小值
来源：http://or.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iv.lnxyls.cn

[Q30] 分组统计
来源：http://ur.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yd.shtwfgs.cn

[Q31] 分组后过滤
来源：http://fw.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fo.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://zz.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kt.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qy.shxzskj.cn

[Q33] 多列分组
来源：http://cz.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iu.lnxyls.cn

[Q34] 每组取第一条
来源：http://cv.szsharing.cn

SELECT * FROM (
来源：http://zg.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oq.asd995.cn

) t WHERE rn = 1;
来源：http://sd.jctech888.com.cn

[Q35] 内连接
来源：http://as.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sj.wgjwhj.cn

[Q36] 左连接
来源：http://xo.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zq.yuexingan06.cn

[Q37] 右连接
来源：http://jf.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://af.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rm.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aj.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://lj.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zk.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ju.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ut.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ms.nicolike.cn

[Q41] 多表连接
来源：http://dn.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hx.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://eb.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://km.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://az.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://ip.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yu.szxytkj.cn

[Q43] 标量子查询
来源：http://nc.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wp.shxzukj.cn

[Q44] IN 子查询
来源：http://mh.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ue.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://gz.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gq.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wd.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fl.shxzukj.cn

[Q47] 与平均值比较
来源：http://wz.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jv.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://rz.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://by.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://pm.asd995.cn

[Q49] 更新单行
来源：http://fi.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ja.hnjuh.cn

[Q50] 批量更新
来源：http://dn.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ep.hnjuh.cn

[Q51] 用子查询更新
来源：http://ne.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sd.asd995.cn

[Q52] 删除指定行
来源：http://gm.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://iu.jctech888.com.cn

[Q53] 按条件删除
来源：http://sv.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lc.jctech888.com.cn

[Q54] 清空表
来源：http://eq.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://gv.asd995.cn

[Q55] 排名（并列占位）
来源：http://cj.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sm.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://ag.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zu.huixinmuqiang.cn

[Q57] 行号
来源：http://tn.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lf.521024.cn

[Q58] 累计求和
来源：http://ec.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hh.yuexingan06.cn

[Q59] 分组内累计
来源：http://te.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ab.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://bm.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ti.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://da.521024.cn

[Q61] 移动平均
来源：http://yc.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fr.newstarts.cn

[Q62] 分组占比
来源：http://yh.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wb.szxytkj.cn

[Q63] 开启事务
来源：http://du.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zo.lnxyls.cn

[Q64] 提交事务
来源：http://bd.asd995.cn

COMMIT;
来源：http://hx.panjiajie.cn

[Q65] 回滚事务
来源：http://hb.asd995.cn

ROLLBACK;
来源：http://dh.shtwfgs.cn

[Q66] 行锁查询
来源：http://mo.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zc.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://uz.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xe.panjiajie.cn

[Q68] 保存点
来源：http://mo.nicolike.cn

SAVEPOINT sp1;
来源：http://pt.shxzukj.cn

ROLLBACK TO sp1;
来源：http://kz.9csxet.cn

[Q69] 查看执行计划
来源：http://tl.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tq.asd995.cn

[Q70] 更新统计信息
来源：http://gk.hnjuh.cn

ANALYZE TABLE users;
来源：http://jk.hnjuh.cn

[Q71] 查看建表语句
来源：http://se.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xn.huixinmuqiang.cn

[Q72] 查看索引
来源：http://vx.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://uo.jctech888.com.cn

[Q73] 查看表状态
来源：http://zn.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://th.newstarts.cn

[Q74] 强制使用索引
来源：http://wo.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ao.shxzskj.cn

[Q75] 日期格式化
来源：http://sk.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://op.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ub.nszjky.cn

[Q76] 按天统计
来源：http://rt.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ai.chemitech.net.cn

[Q77] 时间加减
来源：http://og.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rj.huixinmuqiang.cn

[Q78] 当前时间
来源：http://cn.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ha.newstarts.cn

[Q79] 字符串拼接
来源：http://lb.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jv.colortex.cn


<!-- 参考信息 -->