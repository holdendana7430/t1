代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vp.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://va.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://oj.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://sd.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bm.nszjky.cn

TS:   // 同 JS
来源：http://oe.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://te.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cq.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dv.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://rh.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://bm.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://gj.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wf.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://zu.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ou.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://es.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fz.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jr.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://rb.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://jc.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://pi.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ff.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://ux.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://hf.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xp.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://on.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://ys.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gr.jianghongdianzi.cn

[O06] 使用进程池
来源：http://dk.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ay.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://au.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://iz.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://du.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://st.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gr.nszjky.cn

Ruby: // fork 块
来源：http://sn.panjiajie.cn

C#:   Parallel.For
来源：http://pu.muxihuayi.cn

================================================================================
来源：http://un.nicolike.cn

P. 常用工具函数
来源：http://qc.nszjky.cn

================================================================================
来源：http://il.newstarts.cn

[P01] 生成 UUID
来源：http://zt.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://kg.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uq.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ct.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://bs.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://vz.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://at.colortex.cn

Ruby: SecureRandom.uuid
来源：http://mm.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://gx.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://eg.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ya.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vn.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aq.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://un.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nn.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bf.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sw.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gm.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://eq.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ch.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jc.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://le.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cd.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gg.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lz.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nd.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zx.colortex.cn

[P04] 求长度
来源：http://ll.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xt.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ku.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jh.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://im.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://qm.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://sl.9csxet.cn

Ruby: x.length;  x.size
来源：http://bx.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://br.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://tw.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ms.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xp.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nu.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sx.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ne.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yx.muxihuayi.cn

Ruby: a == b
来源：http://yg.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jc.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://be.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bn.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://lq.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fu.newstarts.cn

TS:   if (x == null) {}
来源：http://ie.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ze.shxzukj.cn

Go:   if x == nil {}
来源：http://tf.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sc.shtwfgs.cn

C#:   if (x is null) {}
来源：http://xp.wgjwhj.cn

[P07] 防抖与节流
来源：http://gf.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ig.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://cm.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qx.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uv.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jy.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vh.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wx.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vm.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://vz.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://js.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xs.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vx.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kt.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://he.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jp.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gv.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rj.chemitech.net.cn

================================================================================
来源：http://hu.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yi.wgjwhj.cn

================================================================================
来源：http://mo.haigaiapp.cn

[Q01] 创建表
来源：http://he.huixinmuqiang.cn

CREATE TABLE users (
来源：http://iw.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gh.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://hp.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://av.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nq.panjiajie.cn

);
来源：http://rh.nszjky.cn

[Q02] 创建带外键的表
来源：http://jl.asd995.cn

CREATE TABLE orders (
来源：http://ym.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qd.newstarts.cn

user_id INT NOT NULL,
来源：http://jl.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://qn.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://if.szsharing.cn

);
来源：http://ox.chemitech.net.cn

[Q03] 增加列
来源：http://gr.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://va.szxytkj.cn

[Q04] 修改列类型
来源：http://ps.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dl.huixinmuqiang.cn

[Q05] 重命名列
来源：http://yg.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vk.9csxet.cn

[Q06] 删除列
来源：http://qv.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qa.muxihuayi.cn

[Q07] 删除表
来源：http://bh.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://bs.nicolike.cn

[Q08] 创建普通索引
来源：http://os.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zs.asd995.cn

[Q09] 创建唯一索引
来源：http://tr.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kp.szsharing.cn

[Q10] 插入单行
来源：http://mi.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pc.gzmigu.cn

[Q11] 一次插入多行
来源：http://pf.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ps.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://ph.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sn.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ra.lnxyls.cn

[Q13] 忽略重复插入
来源：http://dw.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rr.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://nx.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bi.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mx.huanxung.cn

[Q15] 查询全部
来源：http://ql.jianghongdianzi.cn

SELECT * FROM users;
来源：http://nj.chemitech.net.cn

[Q16] 查询指定列
来源：http://hp.chemitech.net.cn

SELECT id, name FROM users;
来源：http://fo.haigaiapp.cn

[Q17] 条件查询
来源：http://lq.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cl.hnjuh.cn

[Q18] 模糊匹配
来源：http://oz.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pb.shxzukj.cn

[Q19] 范围查询
来源：http://tr.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wq.haigaiapp.cn

[Q20] IN 列表
来源：http://rv.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nh.9csxet.cn

[Q21] 空值判断
来源：http://cw.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uu.wgjwhj.cn

[Q22] 排序
来源：http://pe.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fi.huanxung.cn

[Q23] 分页
来源：http://dd.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yt.colortex.cn

[Q24] 去重
来源：http://su.521024.cn

SELECT DISTINCT city FROM users;
来源：http://pl.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://iy.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ei.gzmigu.cn

[Q26] 计数
来源：http://rv.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://md.huanxung.cn

[Q27] 条件计数
来源：http://yy.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qi.shxzskj.cn

[Q28] 求和与平均
来源：http://od.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tg.bookmarksfly.cn

[Q29] 最大最小值
来源：http://zs.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lt.nicolike.cn

[Q30] 分组统计
来源：http://iv.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yu.jctech888.com.cn

[Q31] 分组后过滤
来源：http://wd.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://di.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://hb.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://me.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uz.hahajie.cn

[Q33] 多列分组
来源：http://ga.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rp.huixiangedu.cn

[Q34] 每组取第一条
来源：http://la.bjjhwx.cn

SELECT * FROM (
来源：http://pd.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qa.chemitech.net.cn

) t WHERE rn = 1;
来源：http://jp.hahajie.cn

[Q35] 内连接
来源：http://ui.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://an.newstarts.cn

[Q36] 左连接
来源：http://md.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ic.yuntaijiaju.cn

[Q37] 右连接
来源：http://wx.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zo.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fx.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tp.colortex.cn

[Q39] 自连接（查上下级）
来源：http://wj.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tn.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qo.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sv.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fg.bjjhwx.cn

[Q41] 多表连接
来源：http://wz.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iz.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://xm.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://xi.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://ck.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://av.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ak.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://uv.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gg.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://sn.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bc.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://or.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vx.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sz.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aq.lnxyls.cn

[Q47] 与平均值比较
来源：http://so.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yu.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://se.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ft.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://dm.bjjhwx.cn

[Q49] 更新单行
来源：http://bf.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pf.huixiangedu.cn

[Q50] 批量更新
来源：http://un.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cw.gzmigu.cn

[Q51] 用子查询更新
来源：http://yo.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ck.muxihuayi.cn

[Q52] 删除指定行
来源：http://pt.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://lx.shxzukj.cn

[Q53] 按条件删除
来源：http://fl.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bj.9csxet.cn

[Q54] 清空表
来源：http://ur.hahajie.cn

TRUNCATE TABLE logs;
来源：http://jm.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://is.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qd.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://in.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yi.gzmigu.cn

[Q57] 行号
来源：http://jw.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bf.jctech888.com.cn

[Q58] 累计求和
来源：http://ns.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yw.newstarts.cn

[Q59] 分组内累计
来源：http://pw.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xc.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://yh.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tk.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qb.hnjuh.cn

[Q61] 移动平均
来源：http://fk.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dv.yuntaijiaju.cn

[Q62] 分组占比
来源：http://jh.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oi.haigaiapp.cn

[Q63] 开启事务
来源：http://ap.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hs.lnxyls.cn

[Q64] 提交事务
来源：http://wl.muxihuayi.cn

COMMIT;
来源：http://bg.newstarts.cn

[Q65] 回滚事务
来源：http://fd.lnxyls.cn

ROLLBACK;
来源：http://xf.colortex.cn

[Q66] 行锁查询
来源：http://pj.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xr.hahajie.cn

[Q67] 设置隔离级别
来源：http://ij.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sc.shxzukj.cn

[Q68] 保存点
来源：http://nf.hahajie.cn

SAVEPOINT sp1;
来源：http://rm.gzmigu.cn

ROLLBACK TO sp1;
来源：http://ww.shxzskj.cn

[Q69] 查看执行计划
来源：http://sn.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qg.yuexingan06.cn

[Q70] 更新统计信息
来源：http://tv.wgjwhj.cn

ANALYZE TABLE users;
来源：http://zi.9csxet.cn

[Q71] 查看建表语句
来源：http://er.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qz.chemitech.net.cn

[Q72] 查看索引
来源：http://sv.shxzskj.cn

SHOW INDEX FROM users;
来源：http://qk.bookmarksfly.cn

[Q73] 查看表状态
来源：http://ot.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://og.9csxet.cn

[Q74] 强制使用索引
来源：http://zq.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ee.hnjuh.cn

[Q75] 日期格式化
来源：http://bp.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ua.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sn.yuntaijiaju.cn

[Q76] 按天统计
来源：http://jq.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rn.haigaiapp.cn

[Q77] 时间加减
来源：http://ji.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tj.jctech888.com.cn

[Q78] 当前时间
来源：http://zw.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eh.szsharing.cn

[Q79] 字符串拼接
来源：http://xh.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sx.panjiajie.cn

[Q80] 字符串截取
来源：http://ee.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kn.nicolike.cn

[Q81] 字符串替换
来源：http://se.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://he.haigaiapp.cn


<!-- 参考信息 -->