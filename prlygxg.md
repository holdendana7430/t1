代发 wailian999

TS:   // worker_threads 线程池
来源：http://zn.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fu.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sh.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lm.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vm.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://vh.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://kh.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://oh.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pg.colortex.cn

TS:   // 同 JS
来源：http://hs.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://pa.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jc.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xu.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://ak.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://ox.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://cf.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ti.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://rw.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rq.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fm.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qq.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gi.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://vq.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://pl.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://kr.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://di.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://th.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://pc.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zr.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lk.521024.cn

Ruby: threads.map(&:join)
来源：http://jo.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ie.chemitech.net.cn

[O06] 使用进程池
来源：http://am.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kp.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lq.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://fv.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://gm.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qu.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hi.muxihuayi.cn

Ruby: // fork 块
来源：http://kr.521024.cn

C#:   Parallel.For
来源：http://ou.shxzskj.cn

================================================================================
来源：http://ey.bjjhwx.cn

P. 常用工具函数
来源：http://mq.gzmigu.cn

================================================================================
来源：http://qw.panjiajie.cn

[P01] 生成 UUID
来源：http://cd.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://rh.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pl.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://hq.hahajie.cn

TS:   crypto.randomUUID()
来源：http://zi.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://au.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://fd.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://bv.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://nj.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://ar.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gi.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ui.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qu.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cw.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cp.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ot.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://il.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vp.shxzukj.cn

[P03] 生成短随机字符串
来源：http://px.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ct.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ux.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wj.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rx.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xm.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ar.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qu.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zu.hahajie.cn

[P04] 求长度
来源：http://uv.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eh.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mp.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pg.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hl.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://uv.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://ek.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://uk.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mc.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://ch.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gj.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bs.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hx.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uz.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://og.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xt.newstarts.cn

Ruby: a == b
来源：http://ji.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rd.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sv.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dk.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://jz.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iy.newstarts.cn

TS:   if (x == null) {}
来源：http://iq.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tf.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://vw.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bb.yuexingan06.cn

C#:   if (x is null) {}
来源：http://wx.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ip.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nw.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://eu.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://al.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oy.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ne.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rl.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mk.hahajie.cn

[P08] 处理浮点精度问题
来源：http://ui.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ux.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ro.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wr.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://or.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ld.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zi.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pt.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ix.shxzukj.cn

================================================================================
来源：http://ew.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hd.bookmarksfly.cn

================================================================================
来源：http://vj.chemitech.net.cn

[Q01] 创建表
来源：http://mm.9csxet.cn

CREATE TABLE users (
来源：http://nu.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rz.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://re.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://zb.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://im.jianghongdianzi.cn

);
来源：http://kd.hahajie.cn

[Q02] 创建带外键的表
来源：http://ce.colortex.cn

CREATE TABLE orders (
来源：http://lw.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dy.nicolike.cn

user_id INT NOT NULL,
来源：http://qq.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://hv.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ot.bjjhwx.cn

);
来源：http://or.9csxet.cn

[Q03] 增加列
来源：http://ew.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cd.haigaiapp.cn

[Q04] 修改列类型
来源：http://kb.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aq.szxytkj.cn

[Q05] 重命名列
来源：http://uf.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ku.nszjky.cn

[Q06] 删除列
来源：http://uk.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fa.nszjky.cn

[Q07] 删除表
来源：http://jc.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://ea.lnxyls.cn

[Q08] 创建普通索引
来源：http://cf.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rs.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://mn.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ax.haigaiapp.cn

[Q10] 插入单行
来源：http://ee.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fs.wgjwhj.cn

[Q11] 一次插入多行
来源：http://pp.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wj.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://zm.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ix.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tx.panjiajie.cn

[Q13] 忽略重复插入
来源：http://ep.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gp.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://ib.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vk.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ek.bjjhwx.cn

[Q15] 查询全部
来源：http://mg.muxihuayi.cn

SELECT * FROM users;
来源：http://re.shxzukj.cn

[Q16] 查询指定列
来源：http://cv.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://lp.bookmarksfly.cn

[Q17] 条件查询
来源：http://wo.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eo.szsharing.cn

[Q18] 模糊匹配
来源：http://me.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hw.asd995.cn

[Q19] 范围查询
来源：http://ei.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tb.wgjwhj.cn

[Q20] IN 列表
来源：http://fl.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jd.shxzukj.cn

[Q21] 空值判断
来源：http://rp.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uy.9csxet.cn

[Q22] 排序
来源：http://pf.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://la.huanxung.cn

[Q23] 分页
来源：http://wq.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jn.jctech888.com.cn

[Q24] 去重
来源：http://yq.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://et.shxzskj.cn

[Q25] 只取前 N 条
来源：http://kn.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dc.muxihuayi.cn

[Q26] 计数
来源：http://xc.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://tv.colortex.cn

[Q27] 条件计数
来源：http://uk.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uk.muxihuayi.cn

[Q28] 求和与平均
来源：http://fe.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ya.yuexingan06.cn

[Q29] 最大最小值
来源：http://ng.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fd.huanxung.cn

[Q30] 分组统计
来源：http://yw.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ui.gzmigu.cn

[Q31] 分组后过滤
来源：http://ud.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vd.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://wr.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ff.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://li.jctech888.com.cn

[Q33] 多列分组
来源：http://rg.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ju.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ce.shxzskj.cn

SELECT * FROM (
来源：http://if.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oj.nszjky.cn

) t WHERE rn = 1;
来源：http://go.huixinmuqiang.cn

[Q35] 内连接
来源：http://if.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qe.yuntaijiaju.cn

[Q36] 左连接
来源：http://aa.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uj.yuntaijiaju.cn

[Q37] 右连接
来源：http://cn.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lu.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://so.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nl.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://gs.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nf.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ky.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hk.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nb.shxzskj.cn

[Q41] 多表连接
来源：http://mo.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rc.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://hd.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://jd.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://ft.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://kl.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mj.shtwfgs.cn

[Q43] 标量子查询
来源：http://no.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wq.gzmigu.cn

[Q44] IN 子查询
来源：http://ep.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oc.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://dp.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://td.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fr.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://td.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://wb.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oj.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://yb.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://le.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://hq.9csxet.cn

[Q49] 更新单行
来源：http://vl.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fs.huixinmuqiang.cn

[Q50] 批量更新
来源：http://pa.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nc.gzmigu.cn

[Q51] 用子查询更新
来源：http://xu.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ex.asd995.cn

[Q52] 删除指定行
来源：http://kk.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://he.shxzskj.cn

[Q53] 按条件删除
来源：http://rg.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qy.bjjhwx.cn

[Q54] 清空表
来源：http://tm.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://or.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://sq.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sv.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://ne.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://da.521024.cn

[Q57] 行号
来源：http://wf.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sd.colortex.cn

[Q58] 累计求和
来源：http://bq.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ew.shtwfgs.cn

[Q59] 分组内累计
来源：http://sv.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aa.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://yn.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bl.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dz.shtwfgs.cn

[Q61] 移动平均
来源：http://xc.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zv.wgjwhj.cn

[Q62] 分组占比
来源：http://bq.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xq.hahajie.cn

[Q63] 开启事务
来源：http://wx.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vo.nszjky.cn

[Q64] 提交事务
来源：http://ex.yuntaijiaju.cn

COMMIT;
来源：http://sn.521024.cn

[Q65] 回滚事务
来源：http://sq.huixiangedu.cn

ROLLBACK;
来源：http://sn.szsharing.cn

[Q66] 行锁查询
来源：http://em.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yt.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://jr.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jy.jianghongdianzi.cn

[Q68] 保存点
来源：http://ie.newstarts.cn

SAVEPOINT sp1;
来源：http://oi.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://fs.hahajie.cn

[Q69] 查看执行计划
来源：http://aq.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gu.shxzskj.cn

[Q70] 更新统计信息
来源：http://zr.szxytkj.cn

ANALYZE TABLE users;
来源：http://kt.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://uk.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cw.szsharing.cn

[Q72] 查看索引
来源：http://uw.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://ek.nicolike.cn

[Q73] 查看表状态
来源：http://zk.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://en.9csxet.cn

[Q74] 强制使用索引
来源：http://vs.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dn.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://rg.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dp.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sk.huixinmuqiang.cn

[Q76] 按天统计
来源：http://zf.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mt.yuexingan06.cn

[Q77] 时间加减
来源：http://df.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qu.gzmigu.cn

[Q78] 当前时间
来源：http://nw.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xd.lnxyls.cn

[Q79] 字符串拼接
来源：http://xi.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zx.9csxet.cn


<!-- 参考信息 -->