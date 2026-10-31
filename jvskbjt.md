代发 wailian999

TS:   // worker_threads 线程池
来源：http://xs.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ux.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ve.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pk.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://av.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ou.9csxet.cn

Py:   with lock: shared += 1
来源：http://gd.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fm.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nd.nicolike.cn

TS:   // 同 JS
来源：http://at.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://bf.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jw.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yx.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://wn.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://zy.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://fi.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tv.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://ps.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://as.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://at.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qa.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nl.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://we.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://xg.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://bo.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tv.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://zj.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://sf.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ry.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://br.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://rl.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bu.wgjwhj.cn

[O06] 使用进程池
来源：http://hd.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iz.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://po.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://jg.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://ec.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mq.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wd.szsharing.cn

Ruby: // fork 块
来源：http://xy.shxzukj.cn

C#:   Parallel.For
来源：http://ib.szsharing.cn

================================================================================
来源：http://nl.haigaiapp.cn

P. 常用工具函数
来源：http://vw.huixiangedu.cn

================================================================================
来源：http://vs.bookmarksfly.cn

[P01] 生成 UUID
来源：http://hv.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://mw.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yy.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://is.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://jp.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://zz.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://vt.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://ju.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wm.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://uc.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jn.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qy.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rm.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jn.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://et.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sl.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://td.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fs.szxytkj.cn

[P03] 生成短随机字符串
来源：http://wd.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aw.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ok.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ox.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kq.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vc.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fw.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cm.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tv.wgjwhj.cn

[P04] 求长度
来源：http://xl.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://op.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cy.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bs.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dq.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://bw.asd995.cn

Go:   len(arr);  len(m)
来源：http://oc.colortex.cn

Ruby: x.length;  x.size
来源：http://im.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lq.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://qq.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ql.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://av.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ly.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wb.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ke.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vg.nszjky.cn

Ruby: a == b
来源：http://tt.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://te.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://er.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qe.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://ah.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aa.hahajie.cn

TS:   if (x == null) {}
来源：http://ut.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kl.muxihuayi.cn

Go:   if x == nil {}
来源：http://hy.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://he.huixiangedu.cn

C#:   if (x is null) {}
来源：http://ny.colortex.cn

[P07] 防抖与节流
来源：http://zg.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uq.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://or.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cx.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jf.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xc.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vx.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xy.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ap.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://hk.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cd.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pr.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eb.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pa.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ix.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://va.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fs.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tb.szsharing.cn

================================================================================
来源：http://fg.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oh.shxzskj.cn

================================================================================
来源：http://ul.jianghongdianzi.cn

[Q01] 创建表
来源：http://kq.muxihuayi.cn

CREATE TABLE users (
来源：http://ko.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kr.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://ww.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://tk.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mu.shxzukj.cn

);
来源：http://op.szxytkj.cn

[Q02] 创建带外键的表
来源：http://nb.lnxyls.cn

CREATE TABLE orders (
来源：http://ws.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pv.gzmigu.cn

user_id INT NOT NULL,
来源：http://uj.nszjky.cn

amount DECIMAL(10, 2),
来源：http://cu.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xd.jctech888.com.cn

);
来源：http://px.yuexingan06.cn

[Q03] 增加列
来源：http://sp.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ax.newstarts.cn

[Q04] 修改列类型
来源：http://hd.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://au.muxihuayi.cn

[Q05] 重命名列
来源：http://ql.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fl.newstarts.cn

[Q06] 删除列
来源：http://nz.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gy.gzmigu.cn

[Q07] 删除表
来源：http://ca.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ym.huixiangedu.cn

[Q08] 创建普通索引
来源：http://qn.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kh.521024.cn

[Q09] 创建唯一索引
来源：http://wg.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xr.gzmigu.cn

[Q10] 插入单行
来源：http://cx.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fk.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ud.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qe.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://rp.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://py.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tf.szxytkj.cn

[Q13] 忽略重复插入
来源：http://ht.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aa.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ny.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rv.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xn.haigaiapp.cn

[Q15] 查询全部
来源：http://zb.panjiajie.cn

SELECT * FROM users;
来源：http://sm.newstarts.cn

[Q16] 查询指定列
来源：http://rk.shxzukj.cn

SELECT id, name FROM users;
来源：http://vu.jianghongdianzi.cn

[Q17] 条件查询
来源：http://fw.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vh.newstarts.cn

[Q18] 模糊匹配
来源：http://xa.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uv.shtwfgs.cn

[Q19] 范围查询
来源：http://hu.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://db.jctech888.com.cn

[Q20] IN 列表
来源：http://yp.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hv.huixiangedu.cn

[Q21] 空值判断
来源：http://vm.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ol.chemitech.net.cn

[Q22] 排序
来源：http://iy.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yw.asd995.cn

[Q23] 分页
来源：http://sm.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hj.gzmigu.cn

[Q24] 去重
来源：http://in.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://nd.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://cd.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fl.shxzskj.cn

[Q26] 计数
来源：http://tj.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://fj.jianghongdianzi.cn

[Q27] 条件计数
来源：http://lm.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cr.nszjky.cn

[Q28] 求和与平均
来源：http://ye.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nl.szxytkj.cn

[Q29] 最大最小值
来源：http://mj.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uf.huixinmuqiang.cn

[Q30] 分组统计
来源：http://uj.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ya.lnxyls.cn

[Q31] 分组后过滤
来源：http://xd.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://be.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://zc.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rx.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hv.lnxyls.cn

[Q33] 多列分组
来源：http://dw.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ko.9csxet.cn

[Q34] 每组取第一条
来源：http://ju.shxzskj.cn

SELECT * FROM (
来源：http://gk.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ws.9csxet.cn

) t WHERE rn = 1;
来源：http://qn.shxzukj.cn

[Q35] 内连接
来源：http://kj.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pc.521024.cn

[Q36] 左连接
来源：http://ie.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sl.shxzskj.cn

[Q37] 右连接
来源：http://th.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ha.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xy.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lg.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://lk.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hw.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kw.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gw.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sd.yuntaijiaju.cn

[Q41] 多表连接
来源：http://se.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xb.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://pp.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://qo.asd995.cn

[Q42] 连接条件附加过滤
来源：http://xk.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://co.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qf.jctech888.com.cn

[Q43] 标量子查询
来源：http://kj.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nc.521024.cn

[Q44] IN 子查询
来源：http://sr.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rz.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://gx.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yi.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ap.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://az.szxytkj.cn

[Q47] 与平均值比较
来源：http://qr.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cv.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ux.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jc.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://si.yuntaijiaju.cn

[Q49] 更新单行
来源：http://mg.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fa.521024.cn

[Q50] 批量更新
来源：http://rz.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ov.shxzukj.cn

[Q51] 用子查询更新
来源：http://jx.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bh.huanxung.cn

[Q52] 删除指定行
来源：http://br.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://vt.colortex.cn

[Q53] 按条件删除
来源：http://il.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zj.huixinmuqiang.cn

[Q54] 清空表
来源：http://xi.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://gy.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://wd.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vj.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://yl.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sl.nicolike.cn

[Q57] 行号
来源：http://ek.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rm.panjiajie.cn

[Q58] 累计求和
来源：http://oy.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zb.szxytkj.cn

[Q59] 分组内累计
来源：http://wr.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qd.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://uc.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tr.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ep.yuntaijiaju.cn

[Q61] 移动平均
来源：http://st.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jw.yuexingan06.cn

[Q62] 分组占比
来源：http://es.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iz.9csxet.cn

[Q63] 开启事务
来源：http://gq.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fn.nicolike.cn

[Q64] 提交事务
来源：http://qk.panjiajie.cn

COMMIT;
来源：http://vn.asd995.cn

[Q65] 回滚事务
来源：http://ui.newstarts.cn

ROLLBACK;
来源：http://yg.nszjky.cn

[Q66] 行锁查询
来源：http://mr.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tg.nicolike.cn

[Q67] 设置隔离级别
来源：http://zv.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fw.hnjuh.cn

[Q68] 保存点
来源：http://je.521024.cn

SAVEPOINT sp1;
来源：http://uu.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://ij.colortex.cn

[Q69] 查看执行计划
来源：http://qr.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ha.colortex.cn

[Q70] 更新统计信息
来源：http://rf.huixiangedu.cn

ANALYZE TABLE users;
来源：http://cn.bjjhwx.cn

[Q71] 查看建表语句
来源：http://wh.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kp.asd995.cn

[Q72] 查看索引
来源：http://yh.szxytkj.cn

SHOW INDEX FROM users;
来源：http://sp.shxzskj.cn

[Q73] 查看表状态
来源：http://zd.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ae.bjjhwx.cn

[Q74] 强制使用索引
来源：http://mh.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tb.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://oj.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fz.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pu.lnxyls.cn

[Q76] 按天统计
来源：http://uk.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ul.jctech888.com.cn

[Q77] 时间加减
来源：http://vs.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rz.chemitech.net.cn

[Q78] 当前时间
来源：http://bm.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sy.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://or.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fp.chemitech.net.cn


<!-- 参考信息 -->