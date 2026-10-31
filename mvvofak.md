代发 wailian999

TS:   // worker_threads 线程池
来源：http://tu.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xh.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yr.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ua.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pk.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://tn.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://fb.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://ro.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://di.colortex.cn

TS:   // 同 JS
来源：http://rf.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://li.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rs.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mo.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://fx.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://es.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://gi.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ph.colortex.cn

JS:   async function f() { await g(); }
来源：http://qv.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://km.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vz.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xd.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tq.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://em.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://dl.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://tp.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tz.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://uk.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://av.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ya.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qk.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://ga.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qi.nszjky.cn

[O06] 使用进程池
来源：http://xs.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ej.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mz.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://bz.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://eg.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gy.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xj.colortex.cn

Ruby: // fork 块
来源：http://xd.shxzskj.cn

C#:   Parallel.For
来源：http://cs.9csxet.cn

================================================================================
来源：http://za.wgjwhj.cn

P. 常用工具函数
来源：http://lx.bjjhwx.cn

================================================================================
来源：http://om.yuexingan06.cn

[P01] 生成 UUID
来源：http://yy.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://gj.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ov.521024.cn

JS:   crypto.randomUUID()
来源：http://qx.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://od.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://ip.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://ns.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://hy.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://tf.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://zg.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ud.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uh.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vz.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://th.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://so.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fx.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yq.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://by.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://cc.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mp.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ku.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hn.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nh.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xa.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oo.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ep.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oh.jianghongdianzi.cn

[P04] 求长度
来源：http://fn.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jd.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vl.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nk.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qu.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://qj.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://hd.hnjuh.cn

Ruby: x.length;  x.size
来源：http://nb.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mc.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://ut.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rd.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rq.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fh.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rm.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ty.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ni.yuntaijiaju.cn

Ruby: a == b
来源：http://bs.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vm.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mc.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nn.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://nv.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ml.nszjky.cn

TS:   if (x == null) {}
来源：http://rf.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mq.chemitech.net.cn

Go:   if x == nil {}
来源：http://zc.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://si.bjjhwx.cn

C#:   if (x is null) {}
来源：http://gp.haigaiapp.cn

[P07] 防抖与节流
来源：http://kp.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vl.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ma.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fm.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mv.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bq.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uh.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ls.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://ym.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dr.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cq.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ez.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kc.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://us.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ny.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vc.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vk.shtwfgs.cn

================================================================================
来源：http://zp.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lw.shxzskj.cn

================================================================================
来源：http://uy.haigaiapp.cn

[Q01] 创建表
来源：http://hu.nszjky.cn

CREATE TABLE users (
来源：http://fo.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wd.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://xz.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://mh.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wh.szxytkj.cn

);
来源：http://wf.szxytkj.cn

[Q02] 创建带外键的表
来源：http://in.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://hu.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vs.huanxung.cn

user_id INT NOT NULL,
来源：http://vl.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://qm.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zn.jianghongdianzi.cn

);
来源：http://np.wgjwhj.cn

[Q03] 增加列
来源：http://wm.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gu.hnjuh.cn

[Q04] 修改列类型
来源：http://je.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ru.colortex.cn

[Q05] 重命名列
来源：http://xv.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://la.hahajie.cn

[Q06] 删除列
来源：http://qv.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ja.chemitech.net.cn

[Q07] 删除表
来源：http://jq.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://bf.panjiajie.cn

[Q08] 创建普通索引
来源：http://ck.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ev.hnjuh.cn

[Q09] 创建唯一索引
来源：http://uc.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pj.huixiangedu.cn

[Q10] 插入单行
来源：http://lg.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://or.shxzukj.cn

[Q11] 一次插入多行
来源：http://hl.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kp.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://zt.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tq.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ka.szsharing.cn

[Q13] 忽略重复插入
来源：http://bw.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oo.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://xc.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ji.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gd.colortex.cn

[Q15] 查询全部
来源：http://aw.jctech888.com.cn

SELECT * FROM users;
来源：http://lf.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://zj.gzmigu.cn

SELECT id, name FROM users;
来源：http://sq.bookmarksfly.cn

[Q17] 条件查询
来源：http://cm.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kk.haigaiapp.cn

[Q18] 模糊匹配
来源：http://fu.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sg.huixiangedu.cn

[Q19] 范围查询
来源：http://mj.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ll.muxihuayi.cn

[Q20] IN 列表
来源：http://ty.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qx.hahajie.cn

[Q21] 空值判断
来源：http://cf.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fv.wgjwhj.cn

[Q22] 排序
来源：http://he.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ej.jianghongdianzi.cn

[Q23] 分页
来源：http://tq.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hl.newstarts.cn

[Q24] 去重
来源：http://lv.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://ia.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://mr.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sh.shtwfgs.cn

[Q26] 计数
来源：http://xn.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ky.huanxung.cn

[Q27] 条件计数
来源：http://ec.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mr.chemitech.net.cn

[Q28] 求和与平均
来源：http://qv.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xv.yuexingan06.cn

[Q29] 最大最小值
来源：http://yh.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hx.szsharing.cn

[Q30] 分组统计
来源：http://pi.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cz.wgjwhj.cn

[Q31] 分组后过滤
来源：http://hg.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ju.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://uf.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oh.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kk.szxytkj.cn

[Q33] 多列分组
来源：http://lk.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jt.newstarts.cn

[Q34] 每组取第一条
来源：http://jr.huixiangedu.cn

SELECT * FROM (
来源：http://lg.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qc.wgjwhj.cn

) t WHERE rn = 1;
来源：http://hm.colortex.cn

[Q35] 内连接
来源：http://gn.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ag.panjiajie.cn

[Q36] 左连接
来源：http://ag.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://me.yuexingan06.cn

[Q37] 右连接
来源：http://cp.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ho.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dn.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dz.521024.cn

[Q39] 自连接（查上下级）
来源：http://jm.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ki.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qq.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tb.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vt.hahajie.cn

[Q41] 多表连接
来源：http://nz.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uo.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://xt.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://mr.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://ea.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://ym.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fb.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://lc.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vo.nicolike.cn

[Q44] IN 子查询
来源：http://ur.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://on.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://xv.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ga.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rz.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bp.yuexingan06.cn

[Q47] 与平均值比较
来源：http://se.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qu.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://st.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cy.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://gh.szsharing.cn

[Q49] 更新单行
来源：http://ae.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zr.shtwfgs.cn

[Q50] 批量更新
来源：http://nu.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ab.shxzukj.cn

[Q51] 用子查询更新
来源：http://hg.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rr.nicolike.cn

[Q52] 删除指定行
来源：http://tf.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://pb.colortex.cn

[Q53] 按条件删除
来源：http://kf.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fg.nicolike.cn

[Q54] 清空表
来源：http://ug.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://be.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://nw.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wg.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://xz.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wb.asd995.cn

[Q57] 行号
来源：http://xe.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sq.huixiangedu.cn

[Q58] 累计求和
来源：http://sm.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pm.colortex.cn

[Q59] 分组内累计
来源：http://wr.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ss.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://hb.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iv.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eb.wgjwhj.cn

[Q61] 移动平均
来源：http://nf.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mo.yuntaijiaju.cn

[Q62] 分组占比
来源：http://ef.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qq.muxihuayi.cn

[Q63] 开启事务
来源：http://em.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gn.jctech888.com.cn

[Q64] 提交事务
来源：http://ji.huanxung.cn

COMMIT;
来源：http://zv.9csxet.cn

[Q65] 回滚事务
来源：http://ax.shxzskj.cn

ROLLBACK;
来源：http://ib.muxihuayi.cn

[Q66] 行锁查询
来源：http://ir.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rx.gzmigu.cn

[Q67] 设置隔离级别
来源：http://xx.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://po.haigaiapp.cn

[Q68] 保存点
来源：http://mb.shxzukj.cn

SAVEPOINT sp1;
来源：http://rx.521024.cn

ROLLBACK TO sp1;
来源：http://sj.shxzukj.cn

[Q69] 查看执行计划
来源：http://wi.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ee.lnxyls.cn

[Q70] 更新统计信息
来源：http://yi.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://bb.gzmigu.cn

[Q71] 查看建表语句
来源：http://lr.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qe.panjiajie.cn

[Q72] 查看索引
来源：http://bv.shxzukj.cn

SHOW INDEX FROM users;
来源：http://ki.9csxet.cn

[Q73] 查看表状态
来源：http://ej.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ib.colortex.cn

[Q74] 强制使用索引
来源：http://kq.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hu.jctech888.com.cn

[Q75] 日期格式化
来源：http://ot.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vq.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fh.521024.cn

[Q76] 按天统计
来源：http://jl.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ds.jianghongdianzi.cn

[Q77] 时间加减
来源：http://gi.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fx.huixiangedu.cn

[Q78] 当前时间
来源：http://ol.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qj.colortex.cn

[Q79] 字符串拼接
来源：http://ai.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haigaiapp.cn


<!-- 参考信息 -->