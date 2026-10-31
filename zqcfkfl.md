代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rl.nicolike.cn

[O03] 加锁保护共享数据
来源：http://lc.colortex.cn

Py:   with lock: shared += 1
来源：http://pp.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://xw.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bj.huixinmuqiang.cn

TS:   // 同 JS
来源：http://bs.521024.cn

Java: synchronized (this) { shared++; }
来源：http://ns.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ub.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://to.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://yg.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://nz.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://xs.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ga.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://lj.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://li.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pn.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mc.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nu.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://go.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://kc.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://sd.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gg.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://gw.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://bc.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dd.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://os.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://bp.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bd.lnxyls.cn

[O06] 使用进程池
来源：http://hk.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lk.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://no.521024.cn

JS:   // child_process / cluster 模块
来源：http://zv.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://lk.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mo.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iu.szxytkj.cn

Ruby: // fork 块
来源：http://an.shxzukj.cn

C#:   Parallel.For
来源：http://zt.panjiajie.cn

================================================================================
来源：http://qn.yuntaijiaju.cn

P. 常用工具函数
来源：http://et.bookmarksfly.cn

================================================================================
来源：http://vb.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://ep.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://uq.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ne.newstarts.cn

JS:   crypto.randomUUID()
来源：http://si.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://no.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://po.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://vp.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://cd.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://sq.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://zj.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vg.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hy.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cl.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fn.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://de.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://su.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ry.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fo.newstarts.cn

[P03] 生成短随机字符串
来源：http://bu.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://un.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qm.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qv.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cb.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zb.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cb.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ln.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iw.newstarts.cn

[P04] 求长度
来源：http://ve.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://un.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ws.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ia.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bv.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://yr.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://wo.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://xj.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vu.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://vq.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://le.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mv.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xz.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nf.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ea.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zc.colortex.cn

Ruby: a == b
来源：http://dq.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yz.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zg.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ci.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://wx.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mf.521024.cn

TS:   if (x == null) {}
来源：http://vj.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wv.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://zk.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://av.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://nl.jctech888.com.cn

[P07] 防抖与节流
来源：http://hl.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sc.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://ya.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://de.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hj.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tz.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ke.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ko.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zu.newstarts.cn

[P08] 处理浮点精度问题
来源：http://rc.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ci.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yp.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://il.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sg.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pd.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nc.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zp.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ri.wgjwhj.cn

================================================================================
来源：http://yo.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gt.shtwfgs.cn

================================================================================
来源：http://qv.lnxyls.cn

[Q01] 创建表
来源：http://tx.asd995.cn

CREATE TABLE users (
来源：http://pa.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ih.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://au.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://na.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://if.shxzskj.cn

);
来源：http://vk.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://ry.huanxung.cn

CREATE TABLE orders (
来源：http://sk.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iv.chemitech.net.cn

user_id INT NOT NULL,
来源：http://dj.9csxet.cn

amount DECIMAL(10, 2),
来源：http://ns.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tr.huixinmuqiang.cn

);
来源：http://xc.bjjhwx.cn

[Q03] 增加列
来源：http://vn.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ea.lnxyls.cn

[Q04] 修改列类型
来源：http://hj.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oi.bookmarksfly.cn

[Q05] 重命名列
来源：http://hb.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dn.9csxet.cn

[Q06] 删除列
来源：http://vn.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ck.panjiajie.cn

[Q07] 删除表
来源：http://da.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://yb.shtwfgs.cn

[Q08] 创建普通索引
来源：http://tt.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vg.colortex.cn

[Q09] 创建唯一索引
来源：http://bg.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dg.hnjuh.cn

[Q10] 插入单行
来源：http://yk.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sc.newstarts.cn

[Q11] 一次插入多行
来源：http://az.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nt.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://nj.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dk.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://la.panjiajie.cn

[Q13] 忽略重复插入
来源：http://at.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cm.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://dd.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ws.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ns.colortex.cn

[Q15] 查询全部
来源：http://fo.newstarts.cn

SELECT * FROM users;
来源：http://oz.521024.cn

[Q16] 查询指定列
来源：http://mn.hahajie.cn

SELECT id, name FROM users;
来源：http://ww.yuntaijiaju.cn

[Q17] 条件查询
来源：http://ae.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gc.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://ss.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zn.newstarts.cn

[Q19] 范围查询
来源：http://yj.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://za.yuexingan06.cn

[Q20] IN 列表
来源：http://hx.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eq.hahajie.cn

[Q21] 空值判断
来源：http://vd.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://le.shxzukj.cn

[Q22] 排序
来源：http://zz.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ey.colortex.cn

[Q23] 分页
来源：http://mf.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pr.chemitech.net.cn

[Q24] 去重
来源：http://ay.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://to.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://jr.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wl.gzmigu.cn

[Q26] 计数
来源：http://mf.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://on.asd995.cn

[Q27] 条件计数
来源：http://xb.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yq.nszjky.cn

[Q28] 求和与平均
来源：http://eq.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bd.colortex.cn

[Q29] 最大最小值
来源：http://pq.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ya.bjjhwx.cn

[Q30] 分组统计
来源：http://jh.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xd.colortex.cn

[Q31] 分组后过滤
来源：http://mu.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://un.521024.cn

[Q32] 分组拼接字符串
来源：http://kz.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xy.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hv.yuntaijiaju.cn

[Q33] 多列分组
来源：http://zm.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xc.huanxung.cn

[Q34] 每组取第一条
来源：http://ad.hahajie.cn

SELECT * FROM (
来源：http://ub.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ml.gzmigu.cn

) t WHERE rn = 1;
来源：http://ok.asd995.cn

[Q35] 内连接
来源：http://td.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ix.jctech888.com.cn

[Q36] 左连接
来源：http://sr.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ux.nszjky.cn

[Q37] 右连接
来源：http://qx.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fn.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wh.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cz.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://uq.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zm.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://la.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wv.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ft.szxytkj.cn

[Q41] 多表连接
来源：http://od.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ns.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://op.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://so.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://xx.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://av.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zo.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://mv.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tk.nicolike.cn

[Q44] IN 子查询
来源：http://zp.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bt.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://qy.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zb.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mc.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wm.szxytkj.cn

[Q47] 与平均值比较
来源：http://rh.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qj.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://kc.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yy.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://xt.szsharing.cn

[Q49] 更新单行
来源：http://zi.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ug.newstarts.cn

[Q50] 批量更新
来源：http://do.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mo.hahajie.cn

[Q51] 用子查询更新
来源：http://nn.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fg.szsharing.cn

[Q52] 删除指定行
来源：http://ej.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://xs.lnxyls.cn

[Q53] 按条件删除
来源：http://te.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sj.colortex.cn

[Q54] 清空表
来源：http://ym.hahajie.cn

TRUNCATE TABLE logs;
来源：http://aa.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://ru.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rl.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://kz.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eg.muxihuayi.cn

[Q57] 行号
来源：http://bg.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gk.bookmarksfly.cn

[Q58] 累计求和
来源：http://oh.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rk.shxzskj.cn

[Q59] 分组内累计
来源：http://vq.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ig.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://gp.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pk.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://km.nszjky.cn

[Q61] 移动平均
来源：http://pf.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kq.colortex.cn

[Q62] 分组占比
来源：http://vm.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tk.nszjky.cn

[Q63] 开启事务
来源：http://ev.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pa.asd995.cn

[Q64] 提交事务
来源：http://fh.newstarts.cn

COMMIT;
来源：http://nu.nszjky.cn

[Q65] 回滚事务
来源：http://kg.newstarts.cn

ROLLBACK;
来源：http://kj.jctech888.com.cn

[Q66] 行锁查询
来源：http://nv.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sm.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://eq.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://up.huixinmuqiang.cn

[Q68] 保存点
来源：http://lq.yuexingan06.cn

SAVEPOINT sp1;
来源：http://hn.panjiajie.cn

ROLLBACK TO sp1;
来源：http://nq.shtwfgs.cn

[Q69] 查看执行计划
来源：http://cx.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://py.szsharing.cn

[Q70] 更新统计信息
来源：http://su.newstarts.cn

ANALYZE TABLE users;
来源：http://nw.asd995.cn

[Q71] 查看建表语句
来源：http://zn.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://js.muxihuayi.cn

[Q72] 查看索引
来源：http://vq.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://wf.haigaiapp.cn

[Q73] 查看表状态
来源：http://vr.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dl.asd995.cn

[Q74] 强制使用索引
来源：http://qf.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ms.bookmarksfly.cn

[Q75] 日期格式化
来源：http://rv.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tw.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tc.lnxyls.cn

[Q76] 按天统计
来源：http://sj.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iz.huixiangedu.cn

[Q77] 时间加减
来源：http://ck.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://je.9csxet.cn

[Q78] 当前时间
来源：http://bv.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zn.szsharing.cn

[Q79] 字符串拼接
来源：http://en.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://di.colortex.cn

[Q80] 字符串截取
来源：http://di.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qg.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://qj.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fc.lnxyls.cn


<!-- 参考信息 -->