代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nw.shxzskj.cn

TS:   // 同 JS
来源：http://nu.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://bg.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gm.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sb.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://iz.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://dv.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://fy.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fj.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ah.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vl.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://im.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uw.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yi.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://wk.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://fl.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://vh.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qo.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://nc.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://aw.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kb.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xo.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://wh.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://df.colortex.cn

[O06] 使用进程池
来源：http://hi.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iv.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zs.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://jz.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://bu.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eo.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sj.huanxung.cn

Ruby: // fork 块
来源：http://gw.lnxyls.cn

C#:   Parallel.For
来源：http://yq.bjjhwx.cn

================================================================================
来源：http://xe.jctech888.com.cn

P. 常用工具函数
来源：http://gs.panjiajie.cn

================================================================================
来源：http://ax.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://gg.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://qt.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://da.huanxung.cn

JS:   crypto.randomUUID()
来源：http://bf.521024.cn

TS:   crypto.randomUUID()
来源：http://rz.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://ga.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://tx.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://er.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://jy.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://nx.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mq.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tq.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uj.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ae.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rb.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yq.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mw.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mz.521024.cn

[P03] 生成短随机字符串
来源：http://tm.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jt.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ms.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pb.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ed.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mg.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wg.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wl.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ah.asd995.cn

[P04] 求长度
来源：http://bw.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xp.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://be.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ee.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tb.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://cp.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://um.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://kk.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rm.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://ng.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lq.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hc.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://we.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nh.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://to.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fy.huixiangedu.cn

Ruby: a == b
来源：http://hl.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wb.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uq.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gf.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://tp.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sg.nicolike.cn

TS:   if (x == null) {}
来源：http://vs.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://la.muxihuayi.cn

Go:   if x == nil {}
来源：http://kc.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iy.yuexingan06.cn

C#:   if (x is null) {}
来源：http://re.nszjky.cn

[P07] 防抖与节流
来源：http://py.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jt.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://jy.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xd.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://do.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ro.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ln.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://de.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fw.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://hq.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://io.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dc.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://to.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://il.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mi.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yu.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yu.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ky.nszjky.cn

================================================================================
来源：http://tx.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tt.shxzskj.cn

================================================================================
来源：http://uh.shtwfgs.cn

[Q01] 创建表
来源：http://sf.wgjwhj.cn

CREATE TABLE users (
来源：http://dt.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ob.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://gh.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://yc.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bf.haigaiapp.cn

);
来源：http://uk.shxzukj.cn

[Q02] 创建带外键的表
来源：http://ev.9csxet.cn

CREATE TABLE orders (
来源：http://nf.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nm.gzmigu.cn

user_id INT NOT NULL,
来源：http://lf.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://xu.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hl.521024.cn

);
来源：http://ee.shtwfgs.cn

[Q03] 增加列
来源：http://nb.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ax.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://tt.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mt.jianghongdianzi.cn

[Q05] 重命名列
来源：http://uy.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gz.shxzukj.cn

[Q06] 删除列
来源：http://er.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qw.wgjwhj.cn

[Q07] 删除表
来源：http://co.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://ew.yuexingan06.cn

[Q08] 创建普通索引
来源：http://cz.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://da.asd995.cn

[Q09] 创建唯一索引
来源：http://gd.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kc.shtwfgs.cn

[Q10] 插入单行
来源：http://kw.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mx.nszjky.cn

[Q11] 一次插入多行
来源：http://gv.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bu.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://ci.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pe.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mq.hnjuh.cn

[Q13] 忽略重复插入
来源：http://za.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gg.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://pr.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://js.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://up.shxzukj.cn

[Q15] 查询全部
来源：http://at.gzmigu.cn

SELECT * FROM users;
来源：http://zo.panjiajie.cn

[Q16] 查询指定列
来源：http://hd.huixiangedu.cn

SELECT id, name FROM users;
来源：http://xa.huixiangedu.cn

[Q17] 条件查询
来源：http://jr.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jt.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://qx.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nh.bookmarksfly.cn

[Q19] 范围查询
来源：http://ce.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://af.newstarts.cn

[Q20] IN 列表
来源：http://jx.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yz.yuexingan06.cn

[Q21] 空值判断
来源：http://cs.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tv.521024.cn

[Q22] 排序
来源：http://cx.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gi.szxytkj.cn

[Q23] 分页
来源：http://qd.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eu.bookmarksfly.cn

[Q24] 去重
来源：http://fx.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://jm.9csxet.cn

[Q25] 只取前 N 条
来源：http://xp.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xh.huanxung.cn

[Q26] 计数
来源：http://zj.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://pk.yuntaijiaju.cn

[Q27] 条件计数
来源：http://wb.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fp.haigaiapp.cn

[Q28] 求和与平均
来源：http://me.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pc.bookmarksfly.cn

[Q29] 最大最小值
来源：http://fo.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lj.wgjwhj.cn

[Q30] 分组统计
来源：http://he.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vo.colortex.cn

[Q31] 分组后过滤
来源：http://ke.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cw.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://hn.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zd.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rg.newstarts.cn

[Q33] 多列分组
来源：http://lk.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wm.asd995.cn

[Q34] 每组取第一条
来源：http://nt.nicolike.cn

SELECT * FROM (
来源：http://uv.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://am.panjiajie.cn

) t WHERE rn = 1;
来源：http://yr.lnxyls.cn

[Q35] 内连接
来源：http://ig.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fn.nszjky.cn

[Q36] 左连接
来源：http://qs.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ar.szsharing.cn

[Q37] 右连接
来源：http://hg.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ie.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gi.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://to.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://xf.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://is.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ea.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cp.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lp.shxzskj.cn

[Q41] 多表连接
来源：http://rk.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bk.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://sf.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://of.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://au.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://iz.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gs.gzmigu.cn

[Q43] 标量子查询
来源：http://zl.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ux.yuexingan06.cn

[Q44] IN 子查询
来源：http://xm.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xl.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://eu.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mo.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ql.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rt.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://oe.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ix.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://ub.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ze.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://mz.newstarts.cn

[Q49] 更新单行
来源：http://sb.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://si.bookmarksfly.cn

[Q50] 批量更新
来源：http://gs.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zt.haigaiapp.cn

[Q51] 用子查询更新
来源：http://or.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hv.521024.cn

[Q52] 删除指定行
来源：http://bn.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://vp.huixiangedu.cn

[Q53] 按条件删除
来源：http://ta.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hd.jctech888.com.cn

[Q54] 清空表
来源：http://ww.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://cd.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://sz.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aq.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://qq.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ls.colortex.cn

[Q57] 行号
来源：http://ht.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cw.shxzskj.cn

[Q58] 累计求和
来源：http://sn.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sg.nszjky.cn

[Q59] 分组内累计
来源：http://tm.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://is.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://vg.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qc.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://en.asd995.cn

[Q61] 移动平均
来源：http://gg.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qp.wgjwhj.cn

[Q62] 分组占比
来源：http://ht.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uk.hnjuh.cn

[Q63] 开启事务
来源：http://nc.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ah.muxihuayi.cn

[Q64] 提交事务
来源：http://jb.hnjuh.cn

COMMIT;
来源：http://ts.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://ko.jctech888.com.cn

ROLLBACK;
来源：http://kp.huixiangedu.cn

[Q66] 行锁查询
来源：http://yu.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kz.lnxyls.cn

[Q67] 设置隔离级别
来源：http://lu.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vm.shxzukj.cn

[Q68] 保存点
来源：http://ms.lnxyls.cn

SAVEPOINT sp1;
来源：http://ne.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://in.nszjky.cn

[Q69] 查看执行计划
来源：http://or.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yv.bjjhwx.cn

[Q70] 更新统计信息
来源：http://dg.asd995.cn

ANALYZE TABLE users;
来源：http://tf.huanxung.cn

[Q71] 查看建表语句
来源：http://gd.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://go.asd995.cn

[Q72] 查看索引
来源：http://dp.asd995.cn

SHOW INDEX FROM users;
来源：http://mh.nicolike.cn

[Q73] 查看表状态
来源：http://gj.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bf.521024.cn

[Q74] 强制使用索引
来源：http://cn.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ay.nicolike.cn

[Q75] 日期格式化
来源：http://xz.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://an.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zx.9csxet.cn

[Q76] 按天统计
来源：http://xa.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://he.hahajie.cn

[Q77] 时间加减
来源：http://ca.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bv.wgjwhj.cn

[Q78] 当前时间
来源：http://hq.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://he.chemitech.net.cn

[Q79] 字符串拼接
来源：http://qu.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lp.panjiajie.cn

[Q80] 字符串截取
来源：http://lb.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xa.asd995.cn

[Q81] 字符串替换
来源：http://lt.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nd.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://dq.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://au.muxihuayi.cn

[Q83] 大小写转换
来源：http://eg.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mc.asd995.cn


<!-- 参考信息 -->