代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://vq.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://hz.colortex.cn

[O04] 定义异步函数并等待
来源：http://fs.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://uj.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wz.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://hp.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ep.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yb.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ww.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oh.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://py.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://qc.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://yx.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vn.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://am.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://vi.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ms.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cf.hahajie.cn

Ruby: threads.map(&:join)
来源：http://hq.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gp.521024.cn

[O06] 使用进程池
来源：http://le.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ij.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bb.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://pf.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://dm.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iv.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mj.9csxet.cn

Ruby: // fork 块
来源：http://fv.asd995.cn

C#:   Parallel.For
来源：http://ra.bjjhwx.cn

================================================================================
来源：http://mg.nicolike.cn

P. 常用工具函数
来源：http://by.panjiajie.cn

================================================================================
来源：http://ci.lnxyls.cn

[P01] 生成 UUID
来源：http://yo.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://ai.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bc.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://ur.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://ds.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://ng.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://cl.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://ol.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://in.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://ld.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ow.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uj.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cl.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uo.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ut.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sh.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fo.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://um.521024.cn

[P03] 生成短随机字符串
来源：http://hh.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kb.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cm.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yl.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://up.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ds.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nx.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qj.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oc.huixiangedu.cn

[P04] 求长度
来源：http://xt.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nv.huixiangedu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yj.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fd.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rs.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://um.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://sg.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://pv.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ye.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://re.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://of.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yj.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://he.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dh.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://si.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ot.huixiangedu.cn

Ruby: a == b
来源：http://eo.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://um.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ot.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ed.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://hf.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ke.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://wm.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://on.shxzukj.cn

Go:   if x == nil {}
来源：http://qo.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zp.nicolike.cn

C#:   if (x is null) {}
来源：http://sy.9csxet.cn

[P07] 防抖与节流
来源：http://ka.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dy.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://rh.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qt.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://su.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ds.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cv.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yw.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ei.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://dn.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://td.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ao.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rk.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mb.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ur.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nz.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vs.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://im.szxytkj.cn

================================================================================
来源：http://kr.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://on.huanxung.cn

================================================================================
来源：http://lz.szsharing.cn

[Q01] 创建表
来源：http://jg.szsharing.cn

CREATE TABLE users (
来源：http://wh.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ef.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://rh.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://pv.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ov.nicolike.cn

);
来源：http://ym.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://oi.newstarts.cn

CREATE TABLE orders (
来源：http://mo.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ks.yuexingan06.cn

user_id INT NOT NULL,
来源：http://mr.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://ep.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jt.lnxyls.cn

);
来源：http://pz.9csxet.cn

[Q03] 增加列
来源：http://oh.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wj.asd995.cn

[Q04] 修改列类型
来源：http://hk.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zs.nszjky.cn

[Q05] 重命名列
来源：http://ui.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fz.gzmigu.cn

[Q06] 删除列
来源：http://hu.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xl.muxihuayi.cn

[Q07] 删除表
来源：http://on.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://zi.shxzukj.cn

[Q08] 创建普通索引
来源：http://fc.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://we.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://zj.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ua.jianghongdianzi.cn

[Q10] 插入单行
来源：http://gq.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mj.jctech888.com.cn

[Q11] 一次插入多行
来源：http://ky.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://su.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://if.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qs.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vt.shxzukj.cn

[Q13] 忽略重复插入
来源：http://ll.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uq.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://mc.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wz.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ck.bjjhwx.cn

[Q15] 查询全部
来源：http://ln.yuexingan06.cn

SELECT * FROM users;
来源：http://by.bjjhwx.cn

[Q16] 查询指定列
来源：http://nt.nicolike.cn

SELECT id, name FROM users;
来源：http://na.jianghongdianzi.cn

[Q17] 条件查询
来源：http://ne.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ay.lnxyls.cn

[Q18] 模糊匹配
来源：http://ob.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vt.bjjhwx.cn

[Q19] 范围查询
来源：http://am.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tk.nszjky.cn

[Q20] IN 列表
来源：http://vd.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gf.huixiangedu.cn

[Q21] 空值判断
来源：http://az.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bh.wgjwhj.cn

[Q22] 排序
来源：http://di.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nd.nicolike.cn

[Q23] 分页
来源：http://qj.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aq.hnjuh.cn

[Q24] 去重
来源：http://is.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://hp.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://uv.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xf.huixinmuqiang.cn

[Q26] 计数
来源：http://fx.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://qp.jianghongdianzi.cn

[Q27] 条件计数
来源：http://pu.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rh.huixiangedu.cn

[Q28] 求和与平均
来源：http://ha.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bs.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://sh.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ad.shxzskj.cn

[Q30] 分组统计
来源：http://re.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ih.muxihuayi.cn

[Q31] 分组后过滤
来源：http://it.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fi.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://za.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gu.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tr.hahajie.cn

[Q33] 多列分组
来源：http://ir.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mc.bjjhwx.cn

[Q34] 每组取第一条
来源：http://vm.asd995.cn

SELECT * FROM (
来源：http://gk.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mh.nszjky.cn

) t WHERE rn = 1;
来源：http://sa.colortex.cn

[Q35] 内连接
来源：http://hd.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eb.muxihuayi.cn

[Q36] 左连接
来源：http://sj.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ww.shtwfgs.cn

[Q37] 右连接
来源：http://rk.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wb.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vu.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xw.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://qz.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bl.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pq.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qk.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zf.panjiajie.cn

[Q41] 多表连接
来源：http://xt.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mx.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://nw.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://rq.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://ht.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://po.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ok.szsharing.cn

[Q43] 标量子查询
来源：http://mz.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ib.jctech888.com.cn

[Q44] IN 子查询
来源：http://ar.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kx.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://sm.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mh.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xi.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cv.bjjhwx.cn

[Q47] 与平均值比较
来源：http://dk.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mw.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://vr.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gd.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://bf.shxzukj.cn

[Q49] 更新单行
来源：http://np.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jn.shxzukj.cn

[Q50] 批量更新
来源：http://wd.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kc.hnjuh.cn

[Q51] 用子查询更新
来源：http://zu.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lw.lnxyls.cn

[Q52] 删除指定行
来源：http://kb.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://tg.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://ca.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://va.lnxyls.cn

[Q54] 清空表
来源：http://sr.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://su.newstarts.cn

[Q55] 排名（并列占位）
来源：http://pi.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vb.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://sl.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xe.jianghongdianzi.cn

[Q57] 行号
来源：http://bo.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vt.lnxyls.cn

[Q58] 累计求和
来源：http://yv.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lc.newstarts.cn

[Q59] 分组内累计
来源：http://eo.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://za.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://qg.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mw.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xq.jianghongdianzi.cn

[Q61] 移动平均
来源：http://ka.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nu.huixinmuqiang.cn

[Q62] 分组占比
来源：http://tq.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sg.huixiangedu.cn

[Q63] 开启事务
来源：http://fp.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zq.huixinmuqiang.cn

[Q64] 提交事务
来源：http://hs.jianghongdianzi.cn

COMMIT;
来源：http://wz.nicolike.cn

[Q65] 回滚事务
来源：http://to.muxihuayi.cn

ROLLBACK;
来源：http://uz.nszjky.cn

[Q66] 行锁查询
来源：http://zo.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ly.hnjuh.cn

[Q67] 设置隔离级别
来源：http://xv.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://id.lnxyls.cn

[Q68] 保存点
来源：http://yc.521024.cn

SAVEPOINT sp1;
来源：http://gp.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://pa.nszjky.cn

[Q69] 查看执行计划
来源：http://vb.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zy.panjiajie.cn

[Q70] 更新统计信息
来源：http://ph.szsharing.cn

ANALYZE TABLE users;
来源：http://sk.shxzukj.cn

[Q71] 查看建表语句
来源：http://gu.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ix.newstarts.cn

[Q72] 查看索引
来源：http://us.colortex.cn

SHOW INDEX FROM users;
来源：http://wh.hnjuh.cn

[Q73] 查看表状态
来源：http://cb.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ow.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://de.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://be.newstarts.cn

[Q75] 日期格式化
来源：http://im.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eo.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ww.yuexingan06.cn

[Q76] 按天统计
来源：http://wr.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hh.shxzukj.cn

[Q77] 时间加减
来源：http://ds.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fr.szxytkj.cn

[Q78] 当前时间
来源：http://xx.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://if.nicolike.cn

[Q79] 字符串拼接
来源：http://pp.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rx.nicolike.cn

[Q80] 字符串截取
来源：http://uv.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bp.haigaiapp.cn

[Q81] 字符串替换
来源：http://fr.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yl.asd995.cn

[Q82] 字符长度与字节长度
来源：http://eb.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wp.colortex.cn

[Q83] 大小写转换
来源：http://io.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xq.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://vd.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://zt.chemitech.net.cn

[Q85] 数值取整
来源：http://rg.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ac.chemitech.net.cn


<!-- 参考信息 -->