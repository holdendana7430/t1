代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://ki.muxihuayi.cn

Go:   go f()
来源：http://qf.nszjky.cn

Ruby: Thread.new { f }
来源：http://af.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://jc.shxzskj.cn

[O02] 使用线程池
来源：http://ng.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oo.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://di.521024.cn

JS:   // worker_threads 线程池
来源：http://og.hahajie.cn

TS:   // worker_threads 线程池
来源：http://yt.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pn.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cq.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dx.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lf.nicolike.cn

[O03] 加锁保护共享数据
来源：http://dq.shxzukj.cn

Py:   with lock: shared += 1
来源：http://mv.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ky.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vk.nicolike.cn

TS:   // 同 JS
来源：http://rb.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://rt.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dc.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zu.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://ri.hahajie.cn

[O04] 定义异步函数并等待
来源：http://xn.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://lg.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ti.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ey.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ws.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sd.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hu.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ta.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://si.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://ny.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://mi.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zb.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://rf.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://ck.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mb.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cc.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://jk.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kw.shxzukj.cn

[O06] 使用进程池
来源：http://ue.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qd.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zo.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://ul.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ks.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uu.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mk.huixinmuqiang.cn

Ruby: // fork 块
来源：http://sj.jianghongdianzi.cn

C#:   Parallel.For
来源：http://la.chemitech.net.cn

================================================================================
来源：http://qa.hnjuh.cn

P. 常用工具函数
来源：http://sq.szsharing.cn

================================================================================
来源：http://mm.lnxyls.cn

[P01] 生成 UUID
来源：http://ll.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://vm.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://af.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://up.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://nt.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://sh.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://za.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://am.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://qz.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://fq.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mj.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zj.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gy.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lu.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rf.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gj.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rp.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://tc.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pb.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eo.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://va.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qm.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mn.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://np.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ve.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fj.bjjhwx.cn

[P04] 求长度
来源：http://ni.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rq.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zw.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gx.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dv.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://pk.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://lc.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://in.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zv.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://hi.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lp.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ih.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yy.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hk.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ij.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://am.newstarts.cn

Ruby: a == b
来源：http://ah.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ck.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tg.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bo.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://to.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://re.huanxung.cn

TS:   if (x == null) {}
来源：http://gd.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nl.colortex.cn

Go:   if x == nil {}
来源：http://ay.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tb.newstarts.cn

C#:   if (x is null) {}
来源：http://nb.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://rf.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cf.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://rs.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bm.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ff.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dy.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jc.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vm.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ad.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://br.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xj.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yx.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nz.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ug.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gf.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tq.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sn.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gy.yuexingan06.cn

================================================================================
来源：http://yn.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fi.9csxet.cn

================================================================================
来源：http://uc.szsharing.cn

[Q01] 创建表
来源：http://am.huanxung.cn

CREATE TABLE users (
来源：http://wb.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pz.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://qu.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://oj.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nj.colortex.cn

);
来源：http://jh.521024.cn

[Q02] 创建带外键的表
来源：http://qs.huixiangedu.cn

CREATE TABLE orders (
来源：http://ur.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ug.hnjuh.cn

user_id INT NOT NULL,
来源：http://ft.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://ch.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://df.shtwfgs.cn

);
来源：http://tr.muxihuayi.cn

[Q03] 增加列
来源：http://kx.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://en.hnjuh.cn

[Q04] 修改列类型
来源：http://yw.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://li.huixiangedu.cn

[Q05] 重命名列
来源：http://qm.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ye.9csxet.cn

[Q06] 删除列
来源：http://zm.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jf.521024.cn

[Q07] 删除表
来源：http://in.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://kk.hnjuh.cn

[Q08] 创建普通索引
来源：http://dh.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dc.shxzskj.cn

[Q09] 创建唯一索引
来源：http://nj.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nu.hahajie.cn

[Q10] 插入单行
来源：http://hk.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ho.newstarts.cn

[Q11] 一次插入多行
来源：http://yn.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://te.521024.cn

[Q12] 插入后取自增 ID
来源：http://ew.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yz.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dg.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://lu.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vr.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://aw.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pr.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bc.newstarts.cn

[Q15] 查询全部
来源：http://fn.chemitech.net.cn

SELECT * FROM users;
来源：http://gl.szxytkj.cn

[Q16] 查询指定列
来源：http://mh.muxihuayi.cn

SELECT id, name FROM users;
来源：http://ii.hnjuh.cn

[Q17] 条件查询
来源：http://co.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ze.gzmigu.cn

[Q18] 模糊匹配
来源：http://dv.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://np.shxzskj.cn

[Q19] 范围查询
来源：http://sv.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xo.nszjky.cn

[Q20] IN 列表
来源：http://ij.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zw.chemitech.net.cn

[Q21] 空值判断
来源：http://pq.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lv.muxihuayi.cn

[Q22] 排序
来源：http://op.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nw.nszjky.cn

[Q23] 分页
来源：http://hk.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lf.nicolike.cn

[Q24] 去重
来源：http://iy.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://ze.hnjuh.cn

[Q25] 只取前 N 条
来源：http://uv.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gx.huixiangedu.cn

[Q26] 计数
来源：http://le.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://qb.hnjuh.cn

[Q27] 条件计数
来源：http://nc.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ax.muxihuayi.cn

[Q28] 求和与平均
来源：http://ov.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://li.szxytkj.cn

[Q29] 最大最小值
来源：http://af.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iu.hahajie.cn

[Q30] 分组统计
来源：http://np.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wh.panjiajie.cn

[Q31] 分组后过滤
来源：http://zi.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sa.huanxung.cn

[Q32] 分组拼接字符串
来源：http://be.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xg.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yx.huanxung.cn

[Q33] 多列分组
来源：http://lc.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qd.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://km.nszjky.cn

SELECT * FROM (
来源：http://vb.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iz.szsharing.cn

) t WHERE rn = 1;
来源：http://zj.colortex.cn

[Q35] 内连接
来源：http://fd.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://do.muxihuayi.cn

[Q36] 左连接
来源：http://xp.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://du.yuexingan06.cn

[Q37] 右连接
来源：http://yb.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://po.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jf.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fa.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://pp.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sb.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vk.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bq.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jw.colortex.cn

[Q41] 多表连接
来源：http://br.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dt.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://xa.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://tb.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://jm.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://gc.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tg.huixiangedu.cn

[Q43] 标量子查询
来源：http://mt.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://je.hnjuh.cn

[Q44] IN 子查询
来源：http://by.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bh.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://kn.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hg.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tw.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dl.bjjhwx.cn

[Q47] 与平均值比较
来源：http://ik.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oz.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://iz.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nc.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://lg.bjjhwx.cn

[Q49] 更新单行
来源：http://xa.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oi.huixinmuqiang.cn

[Q50] 批量更新
来源：http://co.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://it.shxzukj.cn

[Q51] 用子查询更新
来源：http://nc.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tj.muxihuayi.cn

[Q52] 删除指定行
来源：http://vl.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://be.hnjuh.cn

[Q53] 按条件删除
来源：http://bs.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qn.huixiangedu.cn

[Q54] 清空表
来源：http://hy.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://be.szsharing.cn

[Q55] 排名（并列占位）
来源：http://si.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mn.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://rn.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zm.colortex.cn

[Q57] 行号
来源：http://hq.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mp.szsharing.cn

[Q58] 累计求和
来源：http://lo.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mm.hahajie.cn

[Q59] 分组内累计
来源：http://vz.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rc.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://op.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lm.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://es.szxytkj.cn

[Q61] 移动平均
来源：http://rw.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xe.shtwfgs.cn

[Q62] 分组占比
来源：http://bb.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://it.jctech888.com.cn

[Q63] 开启事务
来源：http://za.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wl.newstarts.cn

[Q64] 提交事务
来源：http://tn.huixiangedu.cn

COMMIT;
来源：http://vg.muxihuayi.cn

[Q65] 回滚事务
来源：http://sf.shtwfgs.cn

ROLLBACK;
来源：http://ox.521024.cn

[Q66] 行锁查询
来源：http://kr.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mj.shxzukj.cn

[Q67] 设置隔离级别
来源：http://ml.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ra.colortex.cn

[Q68] 保存点
来源：http://ki.nszjky.cn

SAVEPOINT sp1;
来源：http://ge.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://pi.asd995.cn

[Q69] 查看执行计划
来源：http://xx.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bi.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://tb.colortex.cn

ANALYZE TABLE users;
来源：http://yy.shtwfgs.cn

[Q71] 查看建表语句
来源：http://th.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yl.huixiangedu.cn

[Q72] 查看索引
来源：http://ok.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://os.colortex.cn

[Q73] 查看表状态
来源：http://ds.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zl.yuexingan06.cn

[Q74] 强制使用索引
来源：http://aj.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ni.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://jr.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jt.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nt.colortex.cn


<!-- 参考信息 -->