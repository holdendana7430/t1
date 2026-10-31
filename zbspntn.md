代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rx.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://lp.shxzukj.cn

Py:   with lock: shared += 1
来源：http://au.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://bq.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ac.bjjhwx.cn

TS:   // 同 JS
来源：http://ow.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://js.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hh.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wv.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://vw.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://wk.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://zr.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fx.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ln.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wt.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://da.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://er.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yp.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://qk.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://ns.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://fm.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jm.521024.cn

JS:   await Promise.all(tasks)
来源：http://wj.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://dg.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://on.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://no.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://wh.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zs.huanxung.cn

[O06] 使用进程池
来源：http://xi.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qo.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lw.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://kp.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://ox.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ym.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ci.nszjky.cn

Ruby: // fork 块
来源：http://pw.jianghongdianzi.cn

C#:   Parallel.For
来源：http://je.bookmarksfly.cn

================================================================================
来源：http://ez.gzmigu.cn

P. 常用工具函数
来源：http://ea.newstarts.cn

================================================================================
来源：http://db.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://xq.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://eg.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zr.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://ys.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://xu.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://yp.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://ke.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://dd.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://pw.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://rj.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://et.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hj.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kd.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vh.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pt.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sp.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ym.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lo.panjiajie.cn

[P03] 生成短随机字符串
来源：http://rl.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rq.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lo.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fa.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gu.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dx.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wl.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hc.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ws.bookmarksfly.cn

[P04] 求长度
来源：http://tz.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wj.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yb.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ya.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kl.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://ig.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://gs.shxzukj.cn

Ruby: x.length;  x.size
来源：http://ye.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dj.huixiangedu.cn

[P05] 判断两个对象内容是否相等
来源：http://lu.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xk.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nn.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nl.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yv.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rl.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rm.muxihuayi.cn

Ruby: a == b
来源：http://mp.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sc.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wg.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nx.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://ax.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zm.huanxung.cn

TS:   if (x == null) {}
来源：http://dg.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eb.9csxet.cn

Go:   if x == nil {}
来源：http://rp.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xy.asd995.cn

C#:   if (x is null) {}
来源：http://ee.huanxung.cn

[P07] 防抖与节流
来源：http://on.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gi.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://dm.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://za.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gz.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ni.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fi.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xs.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://im.colortex.cn

[P08] 处理浮点精度问题
来源：http://gw.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kq.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://if.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ao.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oc.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hs.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nx.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nz.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lq.yuntaijiaju.cn

================================================================================
来源：http://vs.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vn.lnxyls.cn

================================================================================
来源：http://fh.huixiangedu.cn

[Q01] 创建表
来源：http://ul.szsharing.cn

CREATE TABLE users (
来源：http://yh.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ns.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://rz.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://bc.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ll.shxzskj.cn

);
来源：http://cj.panjiajie.cn

[Q02] 创建带外键的表
来源：http://fc.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://uw.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://id.hnjuh.cn

user_id INT NOT NULL,
来源：http://mp.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://oq.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kb.haigaiapp.cn

);
来源：http://sd.panjiajie.cn

[Q03] 增加列
来源：http://iz.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bt.wgjwhj.cn

[Q04] 修改列类型
来源：http://np.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://do.nicolike.cn

[Q05] 重命名列
来源：http://cf.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yf.nicolike.cn

[Q06] 删除列
来源：http://st.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bv.hahajie.cn

[Q07] 删除表
来源：http://ou.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://bw.nicolike.cn

[Q08] 创建普通索引
来源：http://jr.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mb.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://ow.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zm.9csxet.cn

[Q10] 插入单行
来源：http://vd.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pt.shxzukj.cn

[Q11] 一次插入多行
来源：http://ze.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wd.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://dt.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sw.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://io.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://nf.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eb.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://vx.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kg.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ta.huixiangedu.cn

[Q15] 查询全部
来源：http://oo.hahajie.cn

SELECT * FROM users;
来源：http://yo.jctech888.com.cn

[Q16] 查询指定列
来源：http://fr.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://kw.shtwfgs.cn

[Q17] 条件查询
来源：http://ri.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://de.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://qs.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bv.yuntaijiaju.cn

[Q19] 范围查询
来源：http://kf.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ny.chemitech.net.cn

[Q20] IN 列表
来源：http://kz.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mc.nszjky.cn

[Q21] 空值判断
来源：http://ff.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cj.shxzskj.cn

[Q22] 排序
来源：http://ys.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kc.shxzskj.cn

[Q23] 分页
来源：http://av.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bm.bjjhwx.cn

[Q24] 去重
来源：http://jv.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://if.shxzukj.cn

[Q25] 只取前 N 条
来源：http://sc.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jb.gzmigu.cn

[Q26] 计数
来源：http://ha.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://sw.newstarts.cn

[Q27] 条件计数
来源：http://ln.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ad.yuexingan06.cn

[Q28] 求和与平均
来源：http://sn.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tg.nicolike.cn

[Q29] 最大最小值
来源：http://yy.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ng.yuntaijiaju.cn

[Q30] 分组统计
来源：http://qj.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iu.nszjky.cn

[Q31] 分组后过滤
来源：http://sy.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jj.nicolike.cn

[Q32] 分组拼接字符串
来源：http://ng.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tj.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ha.gzmigu.cn

[Q33] 多列分组
来源：http://nh.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ga.nszjky.cn

[Q34] 每组取第一条
来源：http://ra.shxzukj.cn

SELECT * FROM (
来源：http://va.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cj.szxytkj.cn

) t WHERE rn = 1;
来源：http://fr.panjiajie.cn

[Q35] 内连接
来源：http://sw.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bi.shxzskj.cn

[Q36] 左连接
来源：http://xu.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ig.newstarts.cn

[Q37] 右连接
来源：http://oq.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yx.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ox.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pp.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://tc.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uv.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rm.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cj.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cq.newstarts.cn

[Q41] 多表连接
来源：http://av.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ob.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://cq.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://ls.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://xq.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://dd.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qk.asd995.cn

[Q43] 标量子查询
来源：http://rw.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pc.521024.cn

[Q44] IN 子查询
来源：http://dh.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qk.asd995.cn

[Q45] EXISTS 判断存在
来源：http://cp.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gv.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ds.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ht.shxzukj.cn

[Q47] 与平均值比较
来源：http://hu.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fg.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://lk.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pr.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://ok.chemitech.net.cn

[Q49] 更新单行
来源：http://sx.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://au.yuexingan06.cn

[Q50] 批量更新
来源：http://cs.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vy.hnjuh.cn

[Q51] 用子查询更新
来源：http://uj.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oe.hnjuh.cn

[Q52] 删除指定行
来源：http://dn.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://fw.huanxung.cn

[Q53] 按条件删除
来源：http://pv.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ss.521024.cn

[Q54] 清空表
来源：http://tv.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://qp.colortex.cn

[Q55] 排名（并列占位）
来源：http://yd.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fi.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://id.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xn.shxzukj.cn

[Q57] 行号
来源：http://lu.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://np.yuexingan06.cn

[Q58] 累计求和
来源：http://pj.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vc.chemitech.net.cn

[Q59] 分组内累计
来源：http://ut.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ud.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://dh.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wq.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rh.haigaiapp.cn

[Q61] 移动平均
来源：http://xq.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ml.szsharing.cn

[Q62] 分组占比
来源：http://iy.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sa.colortex.cn

[Q63] 开启事务
来源：http://dv.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gn.lnxyls.cn

[Q64] 提交事务
来源：http://ip.yuntaijiaju.cn

COMMIT;
来源：http://za.nszjky.cn

[Q65] 回滚事务
来源：http://nx.jianghongdianzi.cn

ROLLBACK;
来源：http://xk.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://nm.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fe.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://id.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ru.bookmarksfly.cn

[Q68] 保存点
来源：http://ul.wgjwhj.cn

SAVEPOINT sp1;
来源：http://ug.szxytkj.cn

ROLLBACK TO sp1;
来源：http://kb.muxihuayi.cn

[Q69] 查看执行计划
来源：http://cw.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bs.newstarts.cn

[Q70] 更新统计信息
来源：http://kb.colortex.cn

ANALYZE TABLE users;
来源：http://xh.szsharing.cn

[Q71] 查看建表语句
来源：http://ov.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zr.lnxyls.cn

[Q72] 查看索引
来源：http://ng.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://le.colortex.cn

[Q73] 查看表状态
来源：http://cw.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bc.yuexingan06.cn

[Q74] 强制使用索引
来源：http://jc.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wz.wgjwhj.cn

[Q75] 日期格式化
来源：http://rx.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ak.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fd.chemitech.net.cn

[Q76] 按天统计
来源：http://wl.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ve.nszjky.cn

[Q77] 时间加减
来源：http://kk.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vu.lnxyls.cn

[Q78] 当前时间
来源：http://th.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wi.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://bt.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rd.haigaiapp.cn

[Q80] 字符串截取
来源：http://hn.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dv.yuexingan06.cn

[Q81] 字符串替换
来源：http://ys.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qd.szsharing.cn


<!-- 参考信息 -->