代发 wailian999

TS:   // worker_threads 线程池
来源：http://if.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yw.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tl.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ls.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ss.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://yg.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://rd.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://iz.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://px.yuexingan06.cn

TS:   // 同 JS
来源：http://vc.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://af.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qi.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lt.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ja.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://ga.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://vh.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bi.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://zs.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ks.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ma.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ky.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zr.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://cg.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://qv.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://ke.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ng.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://nr.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://qo.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tw.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zy.hahajie.cn

Ruby: threads.map(&:join)
来源：http://tg.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jl.hahajie.cn

[O06] 使用进程池
来源：http://wf.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cp.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bp.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://nm.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://ei.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hf.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jr.jctech888.com.cn

Ruby: // fork 块
来源：http://uj.bjjhwx.cn

C#:   Parallel.For
来源：http://zz.huixiangedu.cn

================================================================================
来源：http://ka.521024.cn

P. 常用工具函数
来源：http://ma.9csxet.cn

================================================================================
来源：http://po.hahajie.cn

[P01] 生成 UUID
来源：http://bi.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://jg.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gm.521024.cn

JS:   crypto.randomUUID()
来源：http://bh.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://cx.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://yb.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://sk.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://dd.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://iz.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://kq.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://by.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nu.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bw.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rr.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vp.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hl.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fs.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ie.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://pz.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://no.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bd.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oi.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xa.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nj.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kt.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ci.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vi.shxzukj.cn

[P04] 求长度
来源：http://hy.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tt.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cb.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://at.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fs.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://yt.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://gr.nszjky.cn

Ruby: x.length;  x.size
来源：http://vy.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hu.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://nd.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hu.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qe.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pd.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rn.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pw.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://to.huanxung.cn

Ruby: a == b
来源：http://mj.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ib.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qd.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dg.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://ol.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ev.chemitech.net.cn

TS:   if (x == null) {}
来源：http://px.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xa.newstarts.cn

Go:   if x == nil {}
来源：http://fz.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ye.haigaiapp.cn

C#:   if (x is null) {}
来源：http://ei.colortex.cn

[P07] 防抖与节流
来源：http://bv.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gs.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://vg.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ir.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fo.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ek.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ob.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zn.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lw.colortex.cn

[P08] 处理浮点精度问题
来源：http://su.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bd.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gp.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sv.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wd.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pz.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ud.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kg.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ei.chemitech.net.cn

================================================================================
来源：http://pi.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kl.huixinmuqiang.cn

================================================================================
来源：http://rn.yuexingan06.cn

[Q01] 创建表
来源：http://ww.szxytkj.cn

CREATE TABLE users (
来源：http://nt.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://se.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://bz.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://vp.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ks.haigaiapp.cn

);
来源：http://wk.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://pw.chemitech.net.cn

CREATE TABLE orders (
来源：http://gb.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://df.yuexingan06.cn

user_id INT NOT NULL,
来源：http://qr.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://mi.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ss.newstarts.cn

);
来源：http://yw.nszjky.cn

[Q03] 增加列
来源：http://gm.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://za.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://ht.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vz.hnjuh.cn

[Q05] 重命名列
来源：http://ar.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xe.hnjuh.cn

[Q06] 删除列
来源：http://oq.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gq.nszjky.cn

[Q07] 删除表
来源：http://na.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://cy.9csxet.cn

[Q08] 创建普通索引
来源：http://ud.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ex.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://vj.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ms.szsharing.cn

[Q10] 插入单行
来源：http://al.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qe.szsharing.cn

[Q11] 一次插入多行
来源：http://pb.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gq.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://tl.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wc.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eh.lnxyls.cn

[Q13] 忽略重复插入
来源：http://rb.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nv.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://cc.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://in.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tn.bjjhwx.cn

[Q15] 查询全部
来源：http://yg.hnjuh.cn

SELECT * FROM users;
来源：http://go.hnjuh.cn

[Q16] 查询指定列
来源：http://ok.szsharing.cn

SELECT id, name FROM users;
来源：http://os.shxzskj.cn

[Q17] 条件查询
来源：http://wf.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yi.panjiajie.cn

[Q18] 模糊匹配
来源：http://cu.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://st.jianghongdianzi.cn

[Q19] 范围查询
来源：http://zi.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bc.gzmigu.cn

[Q20] IN 列表
来源：http://fm.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zr.hahajie.cn

[Q21] 空值判断
来源：http://bq.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mg.bookmarksfly.cn

[Q22] 排序
来源：http://fd.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nk.nicolike.cn

[Q23] 分页
来源：http://os.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iz.colortex.cn

[Q24] 去重
来源：http://vl.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://oo.huanxung.cn

[Q25] 只取前 N 条
来源：http://vm.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kf.lnxyls.cn

[Q26] 计数
来源：http://iw.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://ob.yuexingan06.cn

[Q27] 条件计数
来源：http://bq.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ly.muxihuayi.cn

[Q28] 求和与平均
来源：http://xz.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gx.yuexingan06.cn

[Q29] 最大最小值
来源：http://cu.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rv.9csxet.cn

[Q30] 分组统计
来源：http://ec.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yx.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://bx.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ut.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://ub.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eo.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gg.szxytkj.cn

[Q33] 多列分组
来源：http://ff.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yw.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://ql.yuntaijiaju.cn

SELECT * FROM (
来源：http://bj.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zc.shxzukj.cn

) t WHERE rn = 1;
来源：http://vm.hnjuh.cn

[Q35] 内连接
来源：http://lh.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zq.szxytkj.cn

[Q36] 左连接
来源：http://ji.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ib.yuexingan06.cn

[Q37] 右连接
来源：http://wj.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rm.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cy.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vj.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://gf.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ea.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ym.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mx.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://th.yuexingan06.cn

[Q41] 多表连接
来源：http://lv.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dl.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://lf.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://bw.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://ox.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://xf.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bu.nszjky.cn

[Q43] 标量子查询
来源：http://rq.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ht.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://ik.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://je.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://os.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fa.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qm.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ac.wgjwhj.cn

[Q47] 与平均值比较
来源：http://ic.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jc.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://cy.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cf.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://mz.hnjuh.cn

[Q49] 更新单行
来源：http://nu.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://in.bookmarksfly.cn

[Q50] 批量更新
来源：http://hs.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rp.hnjuh.cn

[Q51] 用子查询更新
来源：http://an.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://be.9csxet.cn

[Q52] 删除指定行
来源：http://cq.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://hb.nicolike.cn

[Q53] 按条件删除
来源：http://dh.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://il.bookmarksfly.cn

[Q54] 清空表
来源：http://nz.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://fy.9csxet.cn

[Q55] 排名（并列占位）
来源：http://tu.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fp.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://oz.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yt.panjiajie.cn

[Q57] 行号
来源：http://op.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://an.shxzukj.cn

[Q58] 累计求和
来源：http://mt.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gd.panjiajie.cn

[Q59] 分组内累计
来源：http://in.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fs.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://nv.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://si.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nr.9csxet.cn

[Q61] 移动平均
来源：http://wi.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rf.bookmarksfly.cn

[Q62] 分组占比
来源：http://tn.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lk.szxytkj.cn

[Q63] 开启事务
来源：http://av.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gu.huixinmuqiang.cn

[Q64] 提交事务
来源：http://iq.newstarts.cn

COMMIT;
来源：http://sk.chemitech.net.cn

[Q65] 回滚事务
来源：http://tn.szxytkj.cn

ROLLBACK;
来源：http://re.haigaiapp.cn

[Q66] 行锁查询
来源：http://je.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://st.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://zm.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sd.newstarts.cn

[Q68] 保存点
来源：http://vi.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://ms.nszjky.cn

ROLLBACK TO sp1;
来源：http://wx.asd995.cn

[Q69] 查看执行计划
来源：http://rz.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zd.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://rt.wgjwhj.cn

ANALYZE TABLE users;
来源：http://bu.yuexingan06.cn

[Q71] 查看建表语句
来源：http://ho.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vs.asd995.cn

[Q72] 查看索引
来源：http://zb.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://vj.bjjhwx.cn

[Q73] 查看表状态
来源：http://xs.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rf.shxzskj.cn

[Q74] 强制使用索引
来源：http://gc.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://az.bookmarksfly.cn

[Q75] 日期格式化
来源：http://ic.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vt.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://te.asd995.cn

[Q76] 按天统计
来源：http://uv.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qq.shxzukj.cn

[Q77] 时间加减
来源：http://yl.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ie.szxytkj.cn

[Q78] 当前时间
来源：http://cu.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cs.szxytkj.cn

[Q79] 字符串拼接
来源：http://iz.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://if.szsharing.cn


<!-- 参考信息 -->